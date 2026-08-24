# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/task/task-patient-charting.spec.ts >> Task - Patient Charting Verification >> AUT_TSK_121 - Task with selected patient is displayed in Patient Charting section
- Location: tests/web/provider-portal/task/task-patient-charting.spec.ts:28:9

# Error details

```
Error: Task "PatientChart 1787560961109" should appear in Patient Charting Tasks tab

expect(received).toBeTruthy()

Received: false
```

# Page snapshot

```yaml
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
      - group "Platform" [ref=f1e226]:
        - button "RPM" [disabled]
        - button "RTM" [disabled]
        - button "CCM" [pressed] [ref=f1e227] [cursor=pointer]
        - button "PCM" [disabled]
      - generic [ref=f1e228]:
        - generic [ref=f1e235]:
          - generic [ref=f1e236]:
            - generic [ref=f1e237]: Witting, Julius
            - generic [ref=f1e238]:
              - text: Male | 07-02-2024 |
              - generic [ref=f1e239]: CCM - Enrolled 08-24-2026
          - generic [ref=f1e240]:
            - generic [ref=f1e241]: User hasn't logged in
            - button [ref=f1e243] [cursor=pointer]
        - generic [ref=f1e248]:
          - generic [ref=f1e249]:
            - paragraph [ref=f1e250]: Upcoming Appointment
            - paragraph [ref=f1e251]: "-"
          - generic [ref=f1e252]:
            - paragraph [ref=f1e253]: Last Appointment
            - paragraph [ref=f1e254]: "-"
        - generic [ref=f1e258]:
          - generic [ref=f1e259]:
            - paragraph [ref=f1e260]: Global Comment
            - button [ref=f1e261] [cursor=pointer]
          - paragraph [ref=f1e266]: Type Your Comment...
        - button "Text Message" [ref=f1e269] [cursor=pointer]
      - generic [ref=f1e275]:
        - tablist [ref=f1e278]:
          - tab "Chats" [ref=f1e279] [cursor=pointer]
          - tab "Care Plan" [ref=f1e280] [cursor=pointer]
          - tab "Assessment" [ref=f1e281] [cursor=pointer]
          - tab "Tasks" [selected] [ref=f1e282] [cursor=pointer]
          - tab "Documents" [ref=f1e283] [cursor=pointer]
          - tab "Home Exercise" [ref=f1e284] [cursor=pointer]
          - tab "Medical History" [ref=f1e285] [cursor=pointer]
          - tab "Enrollments" [ref=f1e286] [cursor=pointer]
          - tab "Care Team" [ref=f1e287] [cursor=pointer]
          - tab "Training Library" [ref=f1e288] [cursor=pointer]
          - tab "Billing" [ref=f1e289] [cursor=pointer]
          - tab "Summary" [ref=f1e290] [cursor=pointer]
        - generic [ref=f1e292] [cursor=pointer]
      - generic [ref=f1e297]:
        - generic [ref=f1e298]:
          - heading "Task" [level=5] [ref=f1e299]
          - generic [ref=f1e300]:
            - group "view toggle" [ref=f1e301]:
              - button "list view" [pressed] [ref=f1e302] [cursor=pointer]
              - button "calendar view" [ref=f1e305] [cursor=pointer]
            - generic [ref=f1e308]:
              - combobox "ToDo" [ref=f1e309] [cursor=pointer]
              - textbox: ToDo
              - group
            - generic [ref=f1e310]:
              - combobox "Call" [active] [ref=f1e311] [cursor=pointer]
              - textbox: CALL
              - group
            - button "+ Add Task" [ref=f1e312] [cursor=pointer]
        - generic [ref=f1e315]:
          - generic [ref=f1e316]:
            - generic "NO" [ref=f1e318]
            - generic "NAME" [ref=f1e320]
            - generic "SERVICE" [ref=f1e322]
            - generic "TASK" [ref=f1e324]
            - generic "PRIORITY" [ref=f1e326]
            - generic "ASSIGNED TO" [ref=f1e328]
            - generic "DUE DATE" [ref=f1e330]
            - generic "TASK STATUS" [ref=f1e332]
            - generic "COMPLETED DATE" [ref=f1e334]
            - generic "COMPLETED BY" [ref=f1e336]
            - generic "ACTIVITY" [ref=f1e338]
            - generic "ACTION" [ref=f1e340]
          - heading "No data found." [level=6] [ref=f1e342]
  - button [ref=f1e344] [cursor=pointer]
  - button [ref=f1e348] [cursor=pointer]
```

# Test source

```ts
  23  |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  24  |         const patient = await createEnrolledPatient({ state: 'Active', program: 'CCM' });
  25  |         patientName = patient.displayName;
  26  |     });
  27  | 
  28  |     test('AUT_TSK_121 - Task with selected patient is displayed in Patient Charting section', async ({ page }) => {
  29  |         test.setTimeout(360000);
  30  |         Logger.step('Test: Create task for patient Automation,Test and verify in Patient Charting');
  31  | 
  32  |         await taskPage.navigateToTask();
  33  | 
  34  |         // Step 1: Create a task with CCM service for patient "Automation, Test"
  35  |         const timestamp = Date.now();
  36  |         const taskName = `PatientChart ${timestamp}`;
  37  | 
  38  |         await taskPage.createTask({
  39  |             service: 'CCM',
  40  |             patientSearch: patientName,
  41  |             action: 'Call',
  42  |             taskName,
  43  |             priority: 'Medium',
  44  |             dueDateOffset: 5,
  45  |             assigneeSearch: 'John'
  46  |         });
  47  |         Logger.info(`Task "${taskName}" created with CCM service for patient Automation, Test`);
  48  | 
  49  |         // Step 2: Verify task was created in task list
  50  |         await taskPage.uncheckMyTasks();
  51  |         await taskPage.setStatusFilter('All');
  52  |         await taskPage.searchTask(taskName);
  53  | 
  54  |         const taskValues = await taskPage.getColumnValues('TASK', true);
  55  |         expect(taskValues.some(t => t.includes(taskName)), 'Task should exist in task list').toBeTruthy();
  56  |         Logger.info('Task verified in task list');
  57  | 
  58  |         // Step 3: Navigate to Patient Charting via global search
  59  |         Logger.step('Opening patient chart for Automation, Test');
  60  |         const patientChart = new PatientChartPage(page);
  61  |         await patientChart.openPatientChartFromGlobalSearch(patientName);
  62  |         await settle(page, 2000);
  63  | 
  64  |         // Step 4: Select CCM service tab in patient chart
  65  |         Logger.step('Selecting CCM service tab');
  66  |         const ccmTab = page.locator("button:has-text('CCM')").first()
  67  |             .or(page.getByText('CCM', { exact: true }).first());
  68  |         await ccmTab.click();
  69  |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  70  |         await settle(page, 2000);
  71  | 
  72  |         // Step 5: Click on the Tasks tab in patient chart
  73  |         Logger.step('Clicking Tasks tab in patient chart');
  74  |         await page.locator("button:has-text('Tasks'), [role='tab']:has-text('Tasks')").first().click();
  75  |         await settle(page, 2000);
  76  | 
  77  |         // Step 6: Filter by Status = ToDo
  78  |         Logger.step('Filtering by ToDo status in patient charting');
  79  |         const statusDropdown = page.locator("//div[contains(@class,'MuiSelect')]//div[@role='combobox']").first();
  80  |         if (await statusDropdown.isVisible().catch(() => false)) {
  81  |             await statusDropdown.click();
  82  |             await settle(page, 800);
  83  |             await page.getByRole('option', { name: 'ToDo' }).click();
  84  |             await settle(page, 1500);
  85  |             Logger.info('Status filter set to ToDo');
  86  |         }
  87  | 
  88  |         // Step 7: Filter by Action = Call
  89  |         Logger.step('Filtering by Call action in patient charting');
  90  |         const actionDropdown = page.locator("//div[contains(@class,'MuiSelect')]//div[@role='combobox']").last();
  91  |         if (await actionDropdown.isVisible().catch(() => false)) {
  92  |             await actionDropdown.click();
  93  |             await settle(page, 800);
  94  |             await page.getByRole('option', { name: 'Call' }).click();
  95  |             await settle(page, 1500);
  96  |             Logger.info('Action filter set to Call');
  97  |         }
  98  | 
  99  |         // Step 8: Verify task appears in patient charting
  100 |         await waitForLoadingHidden(page);
  101 |         const chartTaskValues = await page.evaluate(() => {
  102 |             const allDivs = Array.from(document.querySelectorAll('div'));
  103 |             const nameDiv = allDivs.find(el => {
  104 |                 const text = el.textContent?.trim().replace(/[▲▼\s]/g, '') || '';
  105 |                 return text === 'NAME' && el.parentElement && el.parentElement.children.length > 5;
  106 |             });
  107 |             if (!nameDiv?.parentElement?.parentElement) return [];
  108 |             const headerRow = nameDiv.parentElement;
  109 |             const headers = Array.from(headerRow.children).map(c => (c.textContent || '').trim().replace(/[▲▼]/g, '').trim());
  110 |             const taskIdx = headers.findIndex(h => h.toUpperCase() === 'TASK');
  111 |             if (taskIdx === -1) return [];
  112 |             const container = headerRow.parentElement!;
  113 |             const rows = Array.from(container.children).slice(1);
  114 |             return rows.map(row => {
  115 |                 const cells = Array.from(row.children);
  116 |                 return cells[taskIdx]?.textContent?.trim() || '';
  117 |             }).filter(t => t.length > 0 && !t.includes('No data found'));
  118 |         });
  119 | 
  120 |         Logger.info(`Tasks in patient charting: ${chartTaskValues.join(', ')}`);
  121 |         expect(chartTaskValues.some(t => t.includes(taskName)),
  122 |             `Task "${taskName}" should appear in Patient Charting Tasks tab`
> 123 |         ).toBeTruthy();
      |           ^ Error: Task "PatientChart 1787560961109" should appear in Patient Charting Tasks tab
  124 | 
  125 |         // Step 9: Verify Service = CCM
  126 |         const chartServiceValues = await page.evaluate(() => {
  127 |             const allDivs = Array.from(document.querySelectorAll('div'));
  128 |             const nameDiv = allDivs.find(el => {
  129 |                 const text = el.textContent?.trim().replace(/[▲▼\s]/g, '') || '';
  130 |                 return text === 'NAME' && el.parentElement && el.parentElement.children.length > 5;
  131 |             });
  132 |             if (!nameDiv?.parentElement?.parentElement) return [];
  133 |             const headerRow = nameDiv.parentElement;
  134 |             const headers = Array.from(headerRow.children).map(c => (c.textContent || '').trim().replace(/[▲▼]/g, '').trim());
  135 |             const svcIdx = headers.findIndex(h => h.toUpperCase() === 'SERVICE');
  136 |             if (svcIdx === -1) return [];
  137 |             const container = headerRow.parentElement!;
  138 |             const rows = Array.from(container.children).slice(1);
  139 |             return rows.map(row => {
  140 |                 const cells = Array.from(row.children);
  141 |                 return cells[svcIdx]?.textContent?.trim() || '';
  142 |             }).filter(t => t.length > 0 && !t.includes('No data found'));
  143 |         });
  144 | 
  145 |         if (chartServiceValues.length > 0) {
  146 |             expect(chartServiceValues[0]?.toUpperCase()).toBe('CCM');
  147 |             Logger.info(`Service in patient charting: ${chartServiceValues[0]} ✓`);
  148 |         }
  149 | 
  150 |         // Step 10: Verify Assigned To = John Doe
  151 |         const chartAssignedValues = await page.evaluate(() => {
  152 |             const allDivs = Array.from(document.querySelectorAll('div'));
  153 |             const nameDiv = allDivs.find(el => {
  154 |                 const text = el.textContent?.trim().replace(/[▲▼\s]/g, '') || '';
  155 |                 return text === 'NAME' && el.parentElement && el.parentElement.children.length > 5;
  156 |             });
  157 |             if (!nameDiv?.parentElement?.parentElement) return [];
  158 |             const headerRow = nameDiv.parentElement;
  159 |             const headers = Array.from(headerRow.children).map(c => (c.textContent || '').trim().replace(/[▲▼]/g, '').trim());
  160 |             const assignIdx = headers.findIndex(h => h.toUpperCase() === 'ASSIGNED TO');
  161 |             if (assignIdx === -1) return [];
  162 |             const container = headerRow.parentElement!;
  163 |             const rows = Array.from(container.children).slice(1);
  164 |             return rows.map(row => {
  165 |                 const cells = Array.from(row.children);
  166 |                 return cells[assignIdx]?.textContent?.trim() || '';
  167 |             }).filter(t => t.length > 0 && !t.includes('No data found'));
  168 |         });
  169 | 
  170 |         if (chartAssignedValues.length > 0) {
  171 |             Logger.info(`Assigned To in patient charting: ${chartAssignedValues[0]}`);
  172 |             expect(chartAssignedValues[0]?.toLowerCase()).toContain('john');
  173 |         }
  174 | 
  175 |         Logger.info(`AUT_TSK_121 PASSED: Task displayed in Patient Charting — CCM → Tasks → ToDo + Call → John Doe`);
  176 |     });
  177 | });
  178 | 
```