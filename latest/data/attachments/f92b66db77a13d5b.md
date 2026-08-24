# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/library/care-plan-patient-chart-sync.spec.ts >> Cross-Module: Care Plan → Patient Chart sync (AUT_CROSS_001) >> Create care plan with Allergies + Medication sections, assign to patient, verify sync in patient chart
- Location: tests/web/provider-portal/library/care-plan-patient-chart-sync.spec.ts:73:9

# Error details

```
TimeoutError: locator.click: Timeout 30000ms exceeded.
Call log:
  - waiting for locator('button:has-text(\'CCM\')').first()
    - locator resolved to <button disabled value="CCM" tabindex="-1" type="button" aria-pressed="false" class="MuiButtonBase-root Mui-disabled MuiToggleButtonGroup-grouped MuiToggleButtonGroup-groupedHorizontal MuiToggleButton-root Mui-disabled MuiToggleButton-sizeMedium MuiToggleButton-primary MuiToggleButtonGroup-grouped MuiToggleButtonGroup-groupedHorizontal MuiToggleButtonGroup-middleButton css-17nvd6n">CCM</button>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is not enabled
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is not enabled
    - retrying click action
      - waiting 100ms
    48 × waiting for element to be visible, enabled and stable
       - element is not enabled
     - retrying click action
       - waiting 500ms

```

# Page snapshot

```yaml
- generic [ref=f1e3]:
  - generic [ref=f1e4]:
    - banner [ref=f1e5]:
      - generic [ref=f1e7]:
        - img "Logo" [ref=f1e9]
        - generic [ref=f1e10]:
          - generic [ref=f1e13]:
            - combobox "Search Patient Name, DOB (MM-DD-YYYY), Phone" [ref=f1e17]
            - button "Open" [ref=f1e19] [cursor=pointer]
            - group
          - button [ref=f1e22] [cursor=pointer]:
            - paragraph [ref=f1e25]: New Patient
          - generic [ref=f1e26]:
            - button [ref=f1e27] [cursor=pointer]
            - button [ref=f1e31] [cursor=pointer]
    - generic [ref=f1e36]:
      - list [ref=f1e38]:
        - generic [ref=f1e39]:
          - generic "Virtual Services" [ref=f1e40]:
            - listitem [ref=f1e41] [cursor=pointer]:
              - generic [ref=f1e45]: Virtual Services
          - list [ref=f1e54]:
            - listitem [ref=f1e56] [cursor=pointer]:
              - generic [ref=f1e57]: Care Team Work List
            - listitem [ref=f1e64] [cursor=pointer]:
              - generic [ref=f1e65]: Enrollments
            - listitem [ref=f1e72] [cursor=pointer]:
              - generic [ref=f1e73]: Patient Assessments
            - generic [ref=f1e79]:
              - listitem [ref=f1e80] [cursor=pointer]:
                - generic [ref=f1e81]: Alerts
              - separator [ref=f1e87]
            - listitem [ref=f1e89] [cursor=pointer]:
              - generic [ref=f1e94]:
                - generic [ref=f1e95]: Tasks
                - generic [ref=f1e96]: "164"
            - generic [ref=f1e97]:
              - listitem [ref=f1e98] [cursor=pointer]:
                - generic [ref=f1e99]: Communications
              - separator [ref=f1e105]
            - generic [ref=f1e106]:
              - listitem [ref=f1e107] [cursor=pointer]:
                - generic [ref=f1e108]: Billing
              - separator [ref=f1e114]
            - generic [ref=f1e115]:
              - listitem [ref=f1e116] [cursor=pointer]:
                - generic [ref=f1e117]: Reports
              - separator [ref=f1e123]
            - listitem [ref=f1e125] [cursor=pointer]:
              - generic [ref=f1e126]: Document Library
            - listitem [ref=f1e133] [cursor=pointer]:
              - generic [ref=f1e134]: CCM Library
            - listitem [ref=f1e141] [cursor=pointer]:
              - generic [ref=f1e142]: PCM Library
            - listitem [ref=f1e149] [cursor=pointer]:
              - generic [ref=f1e150]: RPM Library
            - generic [ref=f1e156]:
              - listitem [ref=f1e157] [cursor=pointer]:
                - generic [ref=f1e158]: RTM Library
              - separator [ref=f1e164]
            - listitem [ref=f1e166] [cursor=pointer]:
              - generic [ref=f1e167]: Training Library
        - generic "Call Center" [ref=f1e174]:
          - listitem [ref=f1e175] [cursor=pointer]:
            - generic [ref=f1e179]: Call Center
        - generic "Revenue Cycle Management" [ref=f1e185]:
          - listitem [ref=f1e186] [cursor=pointer]:
            - generic [ref=f1e190]: Revenue Cycle Management
        - generic "Omni Channel" [ref=f1e196]:
          - listitem [ref=f1e197] [cursor=pointer]:
            - generic [ref=f1e201]: Omni Channel
        - separator [ref=f1e206]
        - listitem [ref=f1e207] [cursor=pointer]:
          - generic [ref=f1e211]: Settings
      - paragraph [ref=f1e215]: Jemes Cory
      - list [ref=f1e217]:
        - listitem [ref=f1e218] [cursor=pointer]:
          - generic [ref=f1e222]: Logout
      - generic "Collapse sidebar":
        - listitem
    - main [ref=f1e223]:
      - generic [ref=f1e225]:
        - generic [ref=f1e227]:
          - tablist [ref=f1e231]:
            - tab "Care Plan" [selected] [ref=f1e232] [cursor=pointer]
            - tab "Quick Pick" [ref=f1e233] [cursor=pointer]
            - tab "Assessment" [ref=f1e234] [cursor=pointer]
            - tab "Templates" [ref=f1e235] [cursor=pointer]
            - tab "Time Logs" [ref=f1e236] [cursor=pointer]
          - generic [ref=f1e238]:
            - generic [ref=f1e239] [cursor=pointer]:
              - checkbox "Show Archived" [ref=f1e241]
              - generic [ref=f1e244]: Show Archived
            - generic [ref=f1e247]:
              - textbox "Type here to search" [active] [ref=f1e251]
              - group
            - button "Create Care Plan" [ref=f1e252] [cursor=pointer]
        - generic [ref=f1e258]:
          - generic [ref=f1e259]:
            - generic "NO" [ref=f1e261]
            - generic "TITLE" [ref=f1e263]
            - generic "CONDITIONS" [ref=f1e265]
            - generic "CREATED DATE & TIME" [ref=f1e267]
            - generic "Created By" [ref=f1e269]
            - generic "Status" [ref=f1e271]
            - generic "ACTION" [ref=f1e273]
          - generic [ref=f1e274]:
            - generic "01" [ref=f1e276] [cursor=pointer]
            - generic "CrossSync-1787560080952" [ref=f1e278] [cursor=pointer]
            - generic "A001" [ref=f1e281]: A001-Chole...
            - generic "08-24-2026, 08:28 AM" [ref=f1e283] [cursor=pointer]
            - generic "PROVIDER" [ref=f1e285] [cursor=pointer]
            - generic "ACTIVE" [ref=f1e287] [cursor=pointer]
            - generic [ref=f1e291] [cursor=pointer]
    - button [ref=f1e295] [cursor=pointer]
    - button [ref=f1e299] [cursor=pointer]
  - alert [ref=f1e302]:
    - generic [ref=f1e306]: CarePlan deleted successfully!
    - button "Close" [ref=f1e308] [cursor=pointer]
```

# Test source

```ts
  1   | import { Browser, Page } from '@playwright/test';
  2   | import { ProviderLoginPage } from '../pages/web/provider-portal/login.page';
  3   | import { PatientChartPage } from '../pages/web/provider-portal/patient-wallet/patient-chart.page';
  4   | import { CCMLibraryPage } from '../pages/web/provider-portal/library/ccm-library.page';
  5   | import { CarePlanPage, CarePlanSectionData } from '../pages/web/provider-portal/library/care-plan.page';
  6   | import { Credentials } from '../config/environment.config';
  7   | import { Logger } from './logger';
  8   | import { PROVIDER_STORAGE_STATE } from '../global-setup';
  9   | 
  10  | /**
  11  |  * Shared helpers for the patient-wallet Care Plan spec files.
  12  |  * These were extracted from the monolithic care-plan-workflow.spec.ts when each
  13  |  * scenario was split into its own file.
  14  |  */
  15  | 
  16  | export async function seedCarePlanTemplate(page: Page, name: string): Promise<void> {
  17  |     const ccmLib = new CCMLibraryPage(page);
  18  |     const carePlan = new CarePlanPage(page);
  19  |     await ccmLib.openCCMLibrary();
  20  |     await ccmLib.openCarePlanSection();
  21  |     const section: CarePlanSectionData = {
  22  |         sectionName: 'Long Term Goals',
  23  |         note: 'Seed note',
  24  |         goalTitle: 'Seed Goal',
  25  |         goalType: 'Single Select',
  26  |     };
  27  |     await carePlan.createMinimalCarePlan('D3190', name, 'Seed header', 'Seed footer', section);
  28  |     Logger.info(`Seed care plan template created: ${name}`);
  29  | }
  30  | 
  31  | export async function handleTimeLogIfPresent(page: Page, noteText: string): Promise<void> {
  32  |     const modal = page.locator("xpath=//*[self::div or self::section][.//*[text()='TIME LOG']]").first();
  33  |     if (!(await modal.isVisible({ timeout: 5000 }).catch(() => false))) return;
  34  | 
  35  |     // The TIME LOG modal arrives pre-valid: Logged By + Logged At + Duration
  36  |     // are pre-filled by the app. Log As and Note are OPTIONAL (no asterisk).
  37  |     // Save is enabled on open. Touching Log As as an autocomplete can commit
  38  |     // an invalid value that disables Save, so we only optionally fill Note
  39  |     // and click Save — keeping the form's default valid state.
  40  |     const note = modal.getByPlaceholder('Enter Note').first();
  41  |     if (await note.isVisible({ timeout: 1500 }).catch(() => false)) {
  42  |         await note.fill(noteText).catch(() => {});
  43  |     }
  44  | 
  45  |     const saveBtn = modal.getByRole('button', { name: 'Save' }).first();
  46  |     await saveBtn.waitFor({ state: 'visible', timeout: 5000 });
  47  |     await saveBtn.click({ force: true });
  48  |     await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  49  |     await page.waitForTimeout(2000);
  50  | }
  51  | 
  52  | export async function stepWizardToFinish(page: Page, maxSteps = 15): Promise<void> {
  53  |     for (let i = 0; i < maxSteps; i++) {
  54  |         const finishBtn = page.getByRole('button', { name: /^Finish$/ }).first();
  55  |         if (await finishBtn.isVisible({ timeout: 2000 }).catch(() => false)) {
  56  |             await finishBtn.click();
  57  |             await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  58  |             await page.waitForTimeout(2000);
  59  |             return;
  60  |         }
  61  |         const nextBtn = page.getByRole('button', { name: /^Next$/ }).first();
  62  |         if (!(await nextBtn.isVisible({ timeout: 2000 }).catch(() => false))) {
  63  |             throw new Error('Wizard stuck — neither Next nor Finish visible');
  64  |         }
  65  |         await nextBtn.scrollIntoViewIfNeeded().catch(() => {});
  66  |         await nextBtn.click({ force: true });
  67  |         await page.waitForTimeout(1500);
  68  |     }
  69  |     throw new Error(`Wizard did not reach Finish within ${maxSteps} steps`);
  70  | }
  71  | 
  72  | export async function assignCarePlanToPatient(page: Page, templateName: string): Promise<void> {
  73  |     Logger.step(`Assigning Care Plan "${templateName}" to patient`);
> 74  |     await page.locator("button:has-text('CCM')").first().click();
      |                                                          ^ TimeoutError: locator.click: Timeout 30000ms exceeded.
  75  |     await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  76  |     await page.waitForTimeout(2000);
  77  |     await page.getByRole('tab', { name: 'Care Plan', exact: true }).click();
  78  |     await page.waitForTimeout(2000);
  79  |     await page.getByRole('button', { name: /Manage Plan/i }).click();
  80  |     await page.waitForTimeout(1500);
  81  |     await page.getByRole('menuitem', { name: /Assign New Care Plan/i }).click();
  82  |     await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  83  |     await page.waitForTimeout(3000);
  84  |     const picker = page.getByRole('combobox', { name: 'Select Care Plan' }).last();
  85  |     await picker.click();
  86  |     await page.waitForTimeout(1500);
  87  |     await page.locator(`[role='option']:has-text("${templateName}"), li:has-text("${templateName}")`).first().click();
  88  |     await page.waitForTimeout(2000);
  89  |     // The Assign Care Plan drawer is an 11-step Stepper wizard (Overview → Long
  90  |     // Term Goals → … → Caregiver Questions). Per the frontend source
  91  |     // (AssignCarePlanDrawerIndex.tsx: `activeStep === steps.length - 1 ? Finish : Next`),
  92  |     // "Finish" ONLY renders on the last step — every earlier step shows "Next".
  93  |     // Previously this clicked Finish directly, so on step 0 there was no Finish
  94  |     // button → 30s timeout → the care plan was never assigned (root cause of
  95  |     // AUT_CP_002 / AUT_CP_015 failing). Step Next→…→Finish instead.
  96  |     await stepWizardToFinish(page);
  97  |     const timeLogModal = page.locator("xpath=//*[self::div or self::section][.//*[text()='TIME LOG']]").first();
  98  |     await timeLogModal.waitFor({ state: 'visible', timeout: 15000 });
  99  |     // TIME LOG arrives pre-valid: Logged By + Logged At + Duration are
  100 |     // pre-filled. Log As and Note are OPTIONAL — touching Log As as an
  101 |     // autocomplete can commit an invalid value that disables Save.
  102 |     // Only optionally fill Note then Save with the form's default state.
  103 |     const note = timeLogModal.getByPlaceholder('Enter Note').first();
  104 |     if (await note.isVisible({ timeout: 1500 }).catch(() => false)) {
  105 |         await note.fill(`Assigned "${templateName}" — 5 minute session.`).catch(() => {});
  106 |     }
  107 |     await timeLogModal.getByRole('button', { name: 'Save' }).first().click();
  108 |     await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  109 |     await page.waitForTimeout(3000);
  110 |     Logger.info(`Assignment complete: "${templateName}"`);
  111 | }
  112 | 
  113 | export async function closeAssignedCarePlan(page: Page, templateName: string): Promise<void> {
  114 |     Logger.step(`Closing assigned Care Plan "${templateName}"`);
  115 |     try {
  116 |         await page.locator("button:has-text('CCM')").first().click();
  117 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  118 |         await page.waitForTimeout(2000);
  119 |         await page.getByRole('tab', { name: 'Care Plan', exact: true }).click();
  120 |         await page.waitForTimeout(2000);
  121 |         const combobox = page.getByRole('combobox', { name: 'Select Care Plan' }).first();
  122 |         await combobox.waitFor({ state: 'visible', timeout: 10000 });
  123 |         await combobox.click();
  124 |         await page.waitForTimeout(1500);
  125 |         const option = page.locator(`[role='option']:has-text("${templateName}"), li:has-text("${templateName}")`).first();
  126 |         await option.waitFor({ state: 'visible', timeout: 10000 });
  127 |         await option.click();
  128 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  129 |         await page.waitForTimeout(2000);
  130 |         const reviewCloseBtn = page.locator("button:has-text('Review & Close')").first();
  131 |         await reviewCloseBtn.waitFor({ state: 'visible', timeout: 10000 });
  132 |         await reviewCloseBtn.click();
  133 |         await page.waitForTimeout(2000);
  134 |         await handleTimeLogIfPresent(page, `Cleanup close: ${templateName}`);
  135 |         const confirmBtn = page.getByRole('button', { name: /^(Yes|Confirm|OK|Close)$/ }).first();
  136 |         if (await confirmBtn.isVisible({ timeout: 2000 }).catch(() => false)) {
  137 |             await confirmBtn.click();
  138 |             await page.waitForTimeout(1500);
  139 |         }
  140 |         Logger.info(`Closed: ${templateName}`);
  141 |     } catch (e) {
  142 |         Logger.info(`Cleanup skip close for "${templateName}" — ${(e as Error).message}`);
  143 |     }
  144 | }
  145 | 
  146 | export async function seedProgressEntryForSection(page: Page): Promise<void> {
  147 |     Logger.step('Seeding progress entries via Modify → Next → answer → Finish');
  148 |     await page.getByRole('button', { name: /Manage Plan/i }).click();
  149 |     await page.waitForTimeout(1500);
  150 |     await page.getByRole('menuitem', { name: /Modify Care Plan/i }).click();
  151 |     await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  152 |     await page.waitForTimeout(3000);
  153 |     const maxSteps = 15;
  154 |     for (let i = 0; i < maxSteps; i++) {
  155 |         const firstChoice = page.locator(
  156 |             "input[type='radio']:not(:checked), input[type='checkbox']:not(:checked)"
  157 |         ).first();
  158 |         if (await firstChoice.isVisible({ timeout: 2000 }).catch(() => false)) {
  159 |             await firstChoice.click({ force: true }).catch(() => {});
  160 |             await page.waitForTimeout(500);
  161 |         }
  162 |         const finishBtn = page.getByRole('button', { name: /^Finish$/ }).first();
  163 |         if (await finishBtn.isVisible({ timeout: 1500 }).catch(() => false)) {
  164 |             await finishBtn.click();
  165 |             await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  166 |             await page.waitForTimeout(2500);
  167 |             break;
  168 |         }
  169 |         const nextBtn = page.getByRole('button', { name: /^Next$/ }).first();
  170 |         if (!(await nextBtn.isVisible({ timeout: 1500 }).catch(() => false))) {
  171 |             throw new Error('Modify wizard stuck — neither Next nor Finish visible');
  172 |         }
  173 |         await nextBtn.scrollIntoViewIfNeeded().catch(() => {});
  174 |         await nextBtn.click({ force: true });
```