# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/care-team-worklist/insurance-sync-enrollment-billing.spec.ts >> Care Team Work List (RTM) — Insurance Data Sync >> insurance data on Enrollment matches the Billing row
- Location: tests/web/provider-portal/care-team-worklist/insurance-sync-enrollment-billing.spec.ts:209:9

# Error details

```
Error: Patient row for Ankunding, Jarred should appear in Billing > Enrollments > RTM

expect(locator).toBeVisible() failed

Locator: locator('//*[normalize-space()="Ankunding, Jarred"]/ancestor::*[count(./*) >= 5][1]').first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Patient row for Ankunding, Jarred should appear in Billing > Enrollments > RTM with timeout 15000ms
  - waiting for locator('//*[normalize-space()="Ankunding, Jarred"]/ancestor::*[count(./*) >= 5][1]').first()

```

```yaml
- banner:
  - img "Logo"
  - combobox "Search Patient Name, DOB (MM-DD-YYYY), Phone"
  - button "Open"
  - button "New Patient":
    - paragraph: New Patient
  - button
  - button
- list:
  - listitem: Virtual Services
  - list:
    - listitem: Care Team Work List
    - listitem: Enrollments
    - listitem: Patient Assessments
    - listitem: Alerts
    - separator
    - listitem: Tasks 164
    - listitem: Communications
    - separator
    - listitem: Billing
    - separator
    - listitem: Reports
    - separator
    - listitem: Document Library
    - listitem: CCM Library
    - listitem: PCM Library
    - listitem: RPM Library
    - listitem: RTM Library
    - separator
    - listitem: Training Library
  - listitem: Call Center
  - listitem: Revenue Cycle Management
  - listitem: Omni Channel
  - separator
  - listitem: Settings
- paragraph: Jemes Cory
- list:
  - listitem: Logout
- listitem
- main:
  - heading "Billing" [level=6]
  - button "Choose date, selected date is Jul 1, 2026"
  - textbox "Select Month": Jul 2026
  - text: Enrollments
  - table "simple table":
    - rowgroup:
      - row "RPM RTM":
        - columnheader:
          - paragraph
        - columnheader "RPM":
          - paragraph: RPM
        - columnheader "RTM":
          - paragraph: RTM
    - rowgroup:
      - row "To Be Billed 0 0":
        - cell "To Be Billed":
          - paragraph: To Be Billed
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
      - row "Submitted 0 0":
        - cell "Submitted":
          - paragraph: Submitted
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
  - text: Monitoring
  - table "simple table":
    - rowgroup:
      - row "RPM RTM":
        - columnheader:
          - paragraph
        - columnheader "RPM":
          - paragraph: RPM
        - columnheader "RTM":
          - paragraph: RTM
    - rowgroup:
      - row "To Be Billed 0 0":
        - cell "To Be Billed":
          - paragraph: To Be Billed
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
      - row "Submitted 0 0":
        - cell "Submitted":
          - paragraph: Submitted
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
  - text: Interaction
  - table "simple table":
    - rowgroup:
      - row "RPM RTM CCM PCM":
        - columnheader:
          - paragraph
        - columnheader "RPM":
          - paragraph: RPM
        - columnheader "RTM":
          - paragraph: RTM
        - columnheader "CCM":
          - paragraph: CCM
        - columnheader "PCM":
          - paragraph: PCM
    - rowgroup:
      - row "To Be Billed 0 0 0 0":
        - cell "To Be Billed":
          - paragraph: To Be Billed
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
      - row "Submitted 0 0 0 0":
        - cell "Submitted":
          - paragraph: Submitted
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
        - cell "0":
          - paragraph: "0"
  - heading "ENROLLMENTS (RTM)" [level=5]
  - textbox "Search Patient": Ankunding
  - textbox "Search By Insurance"
  - checkbox "SelfPay"
  - text: SelfPay
  - combobox "Select": All Providers
  - button "Open"
  - combobox: Claim Status
  - combobox: Paid Status
  - button "Export Billing"
  - checkbox "select all rows"
  - text: NAME ▲ SERVICE CRITERIA ENROLL DATE DIAGNOSIS CODES(ICD) PROVIDER CPT CODE INSURANCE CLAIM NUMBER CLAIM STATUS PAID DATE PAID STATUS ACTION
  - heading "No data found." [level=6]
- button
- button
```

# Test source

```ts
  1   | import { test, expect } from '../../../../fixtures/chart.fixtures';
  2   | import type { Page } from '@playwright/test';
  3   | import { ProviderLoginPage } from '../../../../pages/web/provider-portal/login.page';
  4   | import { PatientChartPage } from '../../../../pages/web/provider-portal/patient-wallet/patient-chart.page';
  5   | import { getEnvironmentConfig } from '../../../../config/environment.config';
  6   | import { Logger } from '../../../../utils/logger';
  7   | 
  8   | // ====================================================================
  9   | // Care Team Work List (RTM) — Insurance Data Sync (Enrollment ↔ Billing)
  10  | //
  11  | // Verifies that the insurance type recorded on a patient's enrollment
  12  | // surfaces in the Billing module's row for the same patient.
  13  | //
  14  | // Flow:
  15  | //   1. Sidebar Billing > Enrollments > RTM bucket → search the patient
  16  | //      → capture the INSURANCE column value
  17  | //   2. Open the patient chart > Enrollments tab → confirm the
  18  | //      enrollment record exists for the patient (the same enrollment
  19  | //      that's billed). Cross-check against any insurance value
  20  | //      rendered in the new-enrollment form.
  21  | //   3. Assert both surfaces report the same insurance value
  22  | //      (or, when the chart side doesn't expose insurance directly,
  23  | //      assert the Billing row carries a non-default insurance value).
  24  | // ====================================================================
  25  | 
  26  | const { providerCredentials, providerPortalUrl } = getEnvironmentConfig();
  27  | 
  28  | async function openBillingSidebar(page: Page): Promise<void> {
  29  |     Logger.step('Navigate to /provider/billing directly');
  30  |     // Direct URL nav avoids sidebar-click interception (drawer backdrops,
  31  |     // SPA route state) — same pattern as MonitoringPage.navigateToMonitoring.
  32  |     const origin = new URL(page.url()).origin;
  33  |     page.once('dialog', (d) => d.accept().catch(() => { /* noop */ }));
  34  |     await page.goto(`${origin}/provider/billing`, { waitUntil: 'domcontentloaded', timeout: 30000 });
  35  |     await page.waitForLoadState('networkidle').catch(() => { /* noop */ });
  36  |     await expect(page.getByText(/^Billing$/, { exact: true }).first())
  37  |         .toBeVisible({ timeout: 15000 });
  38  | }
  39  | 
  40  | /**
  41  |  * Sets the Billing top-right month filter. Falls back to the previous
  42  |  * month if the patient's enrollment date is outside the default current
  43  |  * month — so the row surfaces regardless of when the test runs.
  44  |  */
  45  | async function pickBillingMonth(page: Page, monthYear: string): Promise<void> {
  46  |     Logger.step(`Set Billing month filter to "${monthYear}"`);
  47  |     const monthInput = page.getByPlaceholder('Select Month').first();
  48  |     if (!(await monthInput.isVisible({ timeout: 5000 }).catch(() => false))) {
  49  |         Logger.info('Month filter input not visible — skipping month change');
  50  |         return;
  51  |     }
  52  |     await monthInput.click({ clickCount: 3 });
  53  |     await monthInput.fill(monthYear);
  54  |     await monthInput.press('Enter');
  55  |     await page.waitForLoadState('networkidle').catch(() => { /* noop */ });
  56  | }
  57  | 
  58  | function previousMonthYear(): string {
  59  |     const d = new Date();
  60  |     d.setDate(1); // avoid month-rollover edge cases
  61  |     d.setMonth(d.getMonth() - 1);
  62  |     return d.toLocaleString('en-US', { month: 'short' }) + ' ' + d.getFullYear();
  63  | }
  64  | 
  65  | async function selectBillingSectionProgram(
  66  |     page: Page,
  67  |     section: 'Enrollments' | 'Monitoring' | 'Interaction',
  68  |     program: 'RPM' | 'RTM' | 'CCM' | 'PCM',
  69  | ): Promise<void> {
  70  |     Logger.step(`Click "${program}" cell under "${section}" section`);
  71  |     const cell = page
  72  |         .locator(`xpath=//*[normalize-space(text())="${section}"]/following::*[normalize-space(text())="${program}"][1]`)
  73  |         .first();
  74  |     await cell.waitFor({ state: 'visible', timeout: 15000 });
  75  |     await cell.click();
  76  |     await page.waitForLoadState('networkidle').catch(() => { /* noop */ });
  77  |     await expect(page.getByPlaceholder('Search Patient', { exact: true }).first())
  78  |         .toBeVisible({ timeout: 15000 });
  79  | }
  80  | 
  81  | /**
  82  |  * Reads the Billing > Enrollments > RTM row's INSURANCE column for a patient.
  83  |  * The row layout is `NAME | SERVICE | CRITERIA | ENROLL DATE | DIAGNOSIS |
  84  |  * PROVIDER | CPT CODE | INSURANCE | CLAIM NUMBER | …`. Returns the trimmed
  85  |  * insurance text — typical values: "SelfPay", "Other", or an insurer name.
  86  |  */
  87  | async function readBillingInsurance(page: Page, patientDisplayName: string): Promise<string> {
  88  |     const lastName = patientDisplayName.split(',')[0].trim();
  89  |     const searchInput = page.getByPlaceholder('Search Patient', { exact: true }).first();
  90  |     await searchInput.fill(lastName);
  91  | 
  92  |     // The Billing list isn't an ARIA grid in this build — `getByRole('row')`
  93  |     // returns nothing. Anchor on the patient name text and walk up to the
  94  |     // smallest ancestor that contains the row's cells.
  95  |     const patientRow = page
  96  |         .locator(`xpath=//*[normalize-space()="${patientDisplayName}"]/ancestor::*[count(./*) >= 5][1]`)
  97  |         .first();
  98  |     await expect(patientRow, `Patient row for ${patientDisplayName} should appear in Billing > Enrollments > RTM`)
> 99  |         .toBeVisible({ timeout: 15000 });
      |          ^ Error: Patient row for Ankunding, Jarred should appear in Billing > Enrollments > RTM
  100 | 
  101 |     // Read INSURANCE by structural neighbour, not by regex over
  102 |     // concatenated text. The CPT cell is unambiguous (a 9NNNN code,
  103 |     // always starts with "9"); INSURANCE is the cell IMMEDIATELY AFTER
  104 |     // it. This is robust to column reorders inside the row as long as
  105 |     // the CPT-then-INSURANCE adjacency holds (the platform documents
  106 |     // them as a pair). Replaces the previous regex
  107 |     // `9\d{4}([A-Za-z][\w\s/]*?)…` which silently mis-parsed multi-word
  108 |     // insurers containing hyphens.
  109 |     const insuranceText = await patientRow.evaluate((row) => {
  110 |         const cells = Array.from(row.children);
  111 |         const texts = cells.map((c) => (c.textContent ?? '').trim());
  112 |         // Find the CPT cell — it's a 5-digit code starting with 9
  113 |         // (98xxx / 99xxx). Use a tight regex so we don't match diagnosis
  114 |         // codes or year tokens.
  115 |         const cptIdx = texts.findIndex((t) => /^9\d{4}$/.test(t));
  116 |         if (cptIdx < 0) return '';
  117 |         // INSURANCE cell is the next sibling.
  118 |         return texts[cptIdx + 1] ?? '';
  119 |     });
  120 |     if (!insuranceText) {
  121 |         throw new Error(
  122 |             'INSURANCE cell not found by CPT-neighbour adjacency in Billing > Enrollments > RTM row',
  123 |         );
  124 |     }
  125 |     Logger.info(`INSURANCE cell (next to CPT): "${insuranceText}"`);
  126 |     return insuranceText;
  127 | }
  128 | 
  129 | async function readChartProgramInsuranceHint(page: Page, patientDisplayName: string): Promise<string> {
  130 |     Logger.step('Open patient chart > New Enrollment form to read insurance hint');
  131 |     const chart = new PatientChartPage(page);
  132 |     await chart.openPatientChartFromGlobalSearch(patientDisplayName);
  133 | 
  134 |     // Open the chart's Enrollments tab — the patient's existing enrollments
  135 |     // and the New Enrollment trigger live here. The chart's Enrollments
  136 |     // table doesn't render an "Insurance" column itself, but the New
  137 |     // Enrollment form pre-fills insurance from the patient's profile.
  138 |     const enrollmentsTab = page.getByRole('tab', { name: /^Enrollments$/i }).first();
  139 |     await enrollmentsTab.waitFor({ state: 'visible', timeout: 15000 });
  140 |     await enrollmentsTab.click();
  141 |     await page.waitForLoadState('networkidle').catch(() => { /* noop */ });
  142 | 
  143 |     // Clicking "+ New Enrollment" opens the drawer pre-filled with the
  144 |     // patient's profile data — including the Insurance section.
  145 |     const newEnrollmentBtn = page
  146 |         .getByRole('button', { name: /\+\s*New Enrollment/i })
  147 |         .or(page.locator('//button[contains(., "New Enrollment")]'))
  148 |         .first();
  149 |     await newEnrollmentBtn.waitFor({ state: 'visible', timeout: 10000 });
  150 |     await newEnrollmentBtn.click();
  151 | 
  152 |     // Pick the seeded patient in the drawer's patient combobox.
  153 |     const patientCombo = page.locator(
  154 |         'xpath=//*[@role="combobox" and @aria-label="Search"] | //input[@placeholder="Search"]',
  155 |     ).first();
  156 |     await patientCombo.waitFor({ state: 'visible', timeout: 10000 });
  157 |     await patientCombo.click();
  158 |     await patientCombo.fill(patientDisplayName.split(',')[0].trim());
  159 |     const patientOption = page.locator(`//li[contains(., "${patientDisplayName}")]`).first();
  160 |     await patientOption.waitFor({ state: 'visible', timeout: 10000 });
  161 |     await patientOption.click();
  162 | 
  163 |     // The Insurance section renders the patient's current insurance type/name.
  164 |     // Pick up any text node tied to the "Insurance" label.
  165 |     const insuranceField = page
  166 |         .locator('xpath=//*[contains(translate(normalize-space(.), "INSURANCE", "insurance"), "insurance")][string-length(normalize-space()) < 80][1]/following::input[1]')
  167 |         .first();
  168 |     let insuranceValue = '';
  169 |     if (await insuranceField.isVisible({ timeout: 5000 }).catch(() => false)) {
  170 |         insuranceValue = (await insuranceField.inputValue().catch(() => '')) ?? '';
  171 |     }
  172 |     if (!insuranceValue) {
  173 |         // Fallback: read the Insurance section's visible text.
  174 |         const sectionText = (await page
  175 |             .locator('xpath=//*[normalize-space(text())="Insurance"]/ancestor::*[1]')
  176 |             .first()
  177 |             .textContent({ timeout: 5000 })
  178 |             .catch(() => '')) ?? '';
  179 |         insuranceValue = sectionText.replace(/insurance/gi, '').trim();
  180 |     }
  181 | 
  182 |     // Cancel the drawer so the test doesn't accidentally create a new enrollment.
  183 |     const cancelBtn = page.getByRole('button', { name: /^Cancel$/i }).first();
  184 |     if (await cancelBtn.isVisible({ timeout: 3000 }).catch(() => false)) {
  185 |         await cancelBtn.click();
  186 |         const confirmYes = page.getByRole('button', { name: /Yes|Confirm|Discard/i }).first();
  187 |         if (await confirmYes.isVisible({ timeout: 3000 }).catch(() => false)) {
  188 |             await confirmYes.click();
  189 |         }
  190 |     }
  191 |     await page.locator('.MuiBackdrop-root.MuiModal-backdrop').first()
  192 |         .waitFor({ state: 'hidden', timeout: 8000 })
  193 |         .catch(() => { /* noop */ });
  194 | 
  195 |     return insuranceValue.trim();
  196 | }
  197 | 
  198 | test.describe('Care Team Work List (RTM) — Insurance Data Sync', () => {
  199 |     let loginPage: ProviderLoginPage;
```