# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/patient-wallet/assessment-workflow.spec.ts >> Patient Wallet - Assessment Workflow >> AUT_ASM_001 - should complete the full assessment workflow — submit, status turns green, completion date recorded
- Location: tests/web/provider-portal/patient-wallet/assessment-workflow.spec.ts:43:9

# Error details

```
TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
Call log:
  - waiting for locator('[role=\'row\']:has-text("E2EAsm 1778658429326")').first()

```

# Page snapshot

```yaml
- generic [ref=e3]:
  - generic [ref=e4]:
    - banner [ref=e5]:
      - generic [ref=e7]:
        - img "Logo" [ref=e9]
        - generic [ref=e10]:
          - generic [ref=e13]:
            - img [ref=e15]
            - combobox "Search Patient Name, DOB (MM-DD-YYYY), Phone" [ref=e17]
            - button "Open" [ref=e19] [cursor=pointer]:
              - img [ref=e20]
            - group
          - button "New Patient" [ref=e22] [cursor=pointer]:
            - img [ref=e23]
            - paragraph [ref=e25]: New Patient
          - button [ref=e27] [cursor=pointer]:
            - img [ref=e29]
    - generic [ref=e31]:
      - list [ref=e33]:
        - listitem [ref=e34] [cursor=pointer]:
          - img [ref=e36]
          - generic [ref=e39]: Work List
        - listitem [ref=e40] [cursor=pointer]:
          - img [ref=e42]
          - generic [ref=e45]: Enrollments
        - listitem [ref=e46] [cursor=pointer]:
          - img [ref=e48]
          - generic [ref=e51]: Alerts
        - listitem [ref=e52] [cursor=pointer]:
          - img [ref=e54]
          - generic [ref=e57]:
            - text: Tasks
            - generic [ref=e58]: "310"
        - listitem [ref=e59] [cursor=pointer]:
          - img [ref=e61]
          - generic [ref=e64]: Billing
        - listitem [ref=e65] [cursor=pointer]:
          - img [ref=e67]
          - generic [ref=e70]: Document Library
        - listitem [ref=e71] [cursor=pointer]:
          - img [ref=e73]
          - generic [ref=e76]: RPM Library
        - listitem [ref=e77] [cursor=pointer]:
          - img [ref=e79]
          - generic [ref=e82]: RTM Library
        - listitem [ref=e83] [cursor=pointer]:
          - img [ref=e85]
          - generic [ref=e88]: CCM Library
        - listitem [ref=e89] [cursor=pointer]:
          - img [ref=e91]
          - generic [ref=e94]: PCM Library
        - listitem [ref=e95] [cursor=pointer]:
          - img [ref=e97]
          - generic [ref=e100]: Training Library
        - listitem [ref=e101] [cursor=pointer]:
          - img [ref=e103]
          - generic [ref=e106]: Communications
        - listitem [ref=e107] [cursor=pointer]:
          - img [ref=e109]
          - generic [ref=e112]: Settings
        - listitem [ref=e113] [cursor=pointer]:
          - img [ref=e115]
          - generic [ref=e117]: Logout
      - generic [ref=e118]:
        - paragraph [ref=e119]: chirag kumar
        - paragraph [ref=e120]: chirag.kumar@thinkitive.com
        - generic [ref=e121]:
          - img [ref=e122]
          - paragraph
      - listitem [ref=e125] [cursor=pointer]:
        - img [ref=e127]
    - main [ref=e129]:
      - generic [ref=e131]:
        - generic [ref=e133]:
          - tablist [ref=e136]:
            - tab "Care Plan" [ref=e137] [cursor=pointer]
            - tab "Quick Pick" [ref=e138] [cursor=pointer]
            - tab "Assessment" [selected] [ref=e139] [cursor=pointer]: Assessment
            - tab "Templates" [ref=e140] [cursor=pointer]
            - tab "Time Logs" [ref=e141] [cursor=pointer]
          - generic [ref=e143]:
            - generic [ref=e146]:
              - img [ref=e148]
              - textbox "Type here to search" [active] [ref=e150]
              - group
            - button "Add Assessment" [ref=e151] [cursor=pointer]:
              - img [ref=e152]
              - text: Add Assessment
        - generic [ref=e156]:
          - generic [ref=e157]:
            - generic "NO" [ref=e159]
            - generic "TITLE" [ref=e161]
            - generic "DESCRIPTION" [ref=e163]
            - generic "CREATED DATE & TIME" [ref=e165]
            - generic "CREATED BY" [ref=e167]
            - generic "ASSESSMENT TYPE" [ref=e169]
            - generic "ACTION" [ref=e171]
          - generic [ref=e172]:
            - generic "01" [ref=e174] [cursor=pointer]
            - generic "Automation Assessment" [ref=e176] [cursor=pointer]
            - generic "12-15-2025, 12:49 PM" [ref=e179] [cursor=pointer]
            - generic "PROVIDER" [ref=e181] [cursor=pointer]
            - generic "-" [ref=e183] [cursor=pointer]
            - img [ref=e188] [cursor=pointer]
          - generic [ref=e190]:
            - generic "02" [ref=e192] [cursor=pointer]
            - generic "Test" [ref=e194] [cursor=pointer]
            - generic "04-16-2026, 12:50 PM" [ref=e197] [cursor=pointer]
            - generic "PROVIDER" [ref=e199] [cursor=pointer]
            - generic "Q&A" [ref=e201] [cursor=pointer]
            - img [ref=e206] [cursor=pointer]
          - generic [ref=e208]:
            - generic "03" [ref=e210] [cursor=pointer]
            - generic "test2" [ref=e212] [cursor=pointer]
            - generic "04-16-2026, 01:27 PM" [ref=e215] [cursor=pointer]
            - generic "PROVIDER" [ref=e217] [cursor=pointer]
            - generic "-" [ref=e219] [cursor=pointer]
            - img [ref=e224] [cursor=pointer]
          - generic [ref=e226]:
            - generic "04" [ref=e228] [cursor=pointer]
            - generic "Test2" [ref=e230] [cursor=pointer]
            - generic "test" [ref=e232] [cursor=pointer]
            - generic "04-16-2026, 12:57 PM" [ref=e234] [cursor=pointer]
            - generic "PROVIDER" [ref=e236] [cursor=pointer]
            - generic "Q&A" [ref=e238] [cursor=pointer]
            - img [ref=e243] [cursor=pointer]
          - generic [ref=e245]:
            - generic "05" [ref=e247] [cursor=pointer]
            - generic "testnew" [ref=e249] [cursor=pointer]
            - generic "Test" [ref=e251] [cursor=pointer]
            - generic "04-29-2026, 11:41 AM" [ref=e253] [cursor=pointer]
            - generic "PROVIDER" [ref=e255] [cursor=pointer]
            - generic "Q&A" [ref=e257] [cursor=pointer]
            - img [ref=e262] [cursor=pointer]
          - generic [ref=e264]:
            - generic "06" [ref=e266] [cursor=pointer]
            - generic "ViewAsm 1778658429327" [ref=e268] [cursor=pointer]
            - generic "05-13-2026, 07:47 AM" [ref=e271] [cursor=pointer]
            - generic "PROVIDER" [ref=e273] [cursor=pointer]
            - generic "SURVEY" [ref=e275] [cursor=pointer]
            - img [ref=e280] [cursor=pointer]
  - alert [ref=e282]:
    - img [ref=e284]
    - generic [ref=e286]: Assessment deleted successfully
    - button "Close" [ref=e288] [cursor=pointer]:
      - img [ref=e289]
```

# Test source

```ts
  1   | import { Browser, Page } from '@playwright/test';
  2   | import { ProviderLoginPage } from '../pages/web/provider-portal/login.page';
  3   | import { PatientChartPage } from '../pages/web/provider-portal/patient-wallet/patient-chart.page';
  4   | import { CCMLibraryPage } from '../pages/web/provider-portal/library/ccm-library.page';
  5   | import { AssessmentPage, AssessmentQuestionData } from '../pages/web/provider-portal/library/assessment.page';
  6   | import { Credentials } from '../config/environment.config';
  7   | import { Logger } from './logger';
  8   | 
  9   | /**
  10  |  * Shared helpers for the patient-wallet Assessment spec files.
  11  |  */
  12  | 
  13  | export async function seedAssessmentTemplate(page: Page, name: string): Promise<void> {
  14  |     const ccmLib = new CCMLibraryPage(page);
  15  |     const assessment = new AssessmentPage(page);
  16  |     await ccmLib.openCCMLibrary();
  17  |     await ccmLib.openAssessmentSection();
  18  |     const questions: AssessmentQuestionData[] = [
  19  |         {
  20  |             questionTitle: 'Single select Q',
  21  |             questionType: 'SINGLE_SELECT',
  22  |             options: ['Option A', 'Option B', 'Option C'],
  23  |         },
  24  |         {
  25  |             questionTitle: 'Multi select Q',
  26  |             questionType: 'MULTI_SELECT',
  27  |             options: ['Choice 1', 'Choice 2', 'Choice 3'],
  28  |         },
  29  |     ];
  30  |     await assessment.createAssessment(name, 'SURVEY', 'DAILY', questions);
  31  |     Logger.info(`Seed assessment template created: ${name}`);
  32  | }
  33  | 
  34  | /**
  35  |  * Complete an assigned assessment from the patient chart.
  36  |  *   3-dot icon in the row's ACTION column → "Submit" menu item → drawer opens →
  37  |  *   answer all radios + first checkbox per group → click drawer Submit.
  38  |  */
  39  | export async function completeAssignedAssessment(page: Page, assessmentName: string): Promise<void> {
  40  |     Logger.step(`Completing assigned assessment "${assessmentName}" on patient chart`);
  41  | 
  42  |     const patientChart = new PatientChartPage(page);
  43  |     await patientChart.navigateToAssessmentTab();
  44  |     await patientChart.openCurrentAssessmentFolder();
  45  | 
  46  |     const row = page.locator(`[role='row']:has-text("${assessmentName}")`).first();
> 47  |     await row.waitFor({ state: 'attached', timeout: 15000 });
      |               ^ TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
  48  |     await row.scrollIntoViewIfNeeded();
  49  | 
  50  |     const actionCell = row.locator("[role='gridcell']").last();
  51  |     await actionCell.locator("img, button, svg").first().click({ force: true });
  52  |     await page.waitForTimeout(1500);
  53  | 
  54  |     const submitMenuItem = page.getByRole('menuitem', { name: /^Submit$/i }).first();
  55  |     if (await submitMenuItem.isVisible({ timeout: 5000 }).catch(() => false)) {
  56  |         await submitMenuItem.click();
  57  |     } else {
  58  |         await page.getByRole('button', { name: /^Submit$/ }).first().click();
  59  |     }
  60  |     await page.waitForLoadState('networkidle');
  61  |     await page.waitForTimeout(3000);
  62  | 
  63  |     const radios = page.locator("input[type='radio']:not([disabled])");
  64  |     const rcount = await radios.count();
  65  |     for (let i = 0; i < rcount; i++) {
  66  |         await radios.nth(i).click({ force: true }).catch(() => {});
  67  |         await page.waitForTimeout(150);
  68  |     }
  69  |     const checkbox = page.locator("input[type='checkbox']:not([disabled])").first();
  70  |     if (await checkbox.isVisible({ timeout: 2000 }).catch(() => false)) {
  71  |         await checkbox.click({ force: true }).catch(() => {});
  72  |         await page.waitForTimeout(300);
  73  |     }
  74  | 
  75  |     const drawerSubmit = page.getByRole('button', { name: /^Submit$/ }).last();
  76  |     await drawerSubmit.waitFor({ state: 'visible', timeout: 10000 });
  77  |     await drawerSubmit.click();
  78  |     await page.waitForLoadState('networkidle');
  79  |     await page.waitForTimeout(3000);
  80  |     await page.keyboard.press('Escape').catch(() => {});
  81  |     await page.waitForTimeout(1000);
  82  |     Logger.info(`Assessment "${assessmentName}" submitted`);
  83  | }
  84  | 
  85  | /**
  86  |  * Self-contained setup: seed an Assessment template + assign it to the patient.
  87  |  */
  88  | export async function setupAssignedAssessment(
  89  |     browser: Browser,
  90  |     creds: Credentials,
  91  |     portalUrl: string,
  92  |     patientName: string,
  93  |     assessmentName: string
  94  | ): Promise<void> {
  95  |     const ctx = await browser.newContext();
  96  |     const page = await ctx.newPage();
  97  |     const login = new ProviderLoginPage(page);
  98  |     const assessment = new AssessmentPage(page);
  99  |     try {
  100 |         await page.goto(portalUrl);
  101 |         await login.login(creds.username, creds.password);
  102 |         await page.waitForLoadState('networkidle');
  103 |         await seedAssessmentTemplate(page, assessmentName);
  104 |         await assessment.assignAssessment(assessmentName, patientName);
  105 |         await page.waitForTimeout(2000);
  106 |     } finally {
  107 |         await ctx.close();
  108 |     }
  109 | }
  110 | 
  111 | /**
  112 |  * Self-contained cleanup: delete the assessment template from CCM Library.
  113 |  */
  114 | export async function teardownAssessmentTemplate(
  115 |     browser: Browser,
  116 |     creds: Credentials,
  117 |     portalUrl: string,
  118 |     assessmentName: string
  119 | ): Promise<void> {
  120 |     const ctx = await browser.newContext();
  121 |     const page = await ctx.newPage();
  122 |     const login = new ProviderLoginPage(page);
  123 |     const ccmLib = new CCMLibraryPage(page);
  124 |     const assessment = new AssessmentPage(page);
  125 |     try {
  126 |         await page.goto(portalUrl);
  127 |         await login.login(creds.username, creds.password);
  128 |         await page.waitForLoadState('networkidle');
  129 |         await ccmLib.openCCMLibrary();
  130 |         await ccmLib.openAssessmentSection();
  131 |         try { await assessment.deleteAssessment(assessmentName); Logger.info(`Deleted assessment: ${assessmentName}`); }
  132 |         catch (e) { Logger.info(`Cleanup skip "${assessmentName}" — ${(e as Error).message}`); }
  133 |     } finally {
  134 |         await ctx.close();
  135 |     }
  136 | }
  137 | 
  138 | /**
  139 |  * beforeEach helper: login → global search patient → CCM tab.
  140 |  */
  141 | export async function navigateToPatientCcm(page: Page, creds: Credentials, portalUrl: string, patientName: string): Promise<void> {
  142 |     const login = new ProviderLoginPage(page);
  143 |     const patientChart = new PatientChartPage(page);
  144 |     await page.goto(portalUrl);
  145 |     await login.login(creds.username, creds.password);
  146 |     await page.waitForLoadState('networkidle');
  147 |     await patientChart.openPatientChartFromGlobalSearch(patientName);
```