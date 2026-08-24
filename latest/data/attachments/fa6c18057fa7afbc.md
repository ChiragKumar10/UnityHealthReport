# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/care-team-worklist/vitals-sync-rtm.spec.ts >> Care Team Work List (RTM) — Vitals Sync with Patient Chart >> vital recorded on patient chart syncs to Care Team Work List Monitoring
- Location: tests/web/provider-portal/care-team-worklist/vitals-sync-rtm.spec.ts:56:9

# Error details

```
Error: Care Team Work List should show Pain Scale = 15 synced from the chart

Care Team Work List should show Pain Scale = 15 synced from the chart

expect(received).toBe(expected) // Object.is equality

Expected: true
Received: false

Call Log:
- Timeout 90000ms exceeded while waiting on the predicate
```

# Page snapshot

```yaml
- generic [ref=f8e4]:
  - banner [ref=f8e5]:
    - generic [ref=f8e7]:
      - img "Logo" [ref=f8e9]
      - generic [ref=f8e10]:
        - generic [ref=f8e13]:
          - combobox "Search Patient Name, DOB (MM-DD-YYYY), Phone" [ref=f8e17]
          - button "Open" [ref=f8e19] [cursor=pointer]
          - group
        - button [ref=f8e22] [cursor=pointer]:
          - paragraph [ref=f8e25]: New Patient
        - generic [ref=f8e26]:
          - button [ref=f8e27] [cursor=pointer]
          - button [ref=f8e31] [cursor=pointer]
  - generic [ref=f8e36]:
    - list [ref=f8e38]:
      - generic [ref=f8e39]:
        - generic "Virtual Services" [ref=f8e40]:
          - listitem [ref=f8e41] [cursor=pointer]:
            - generic [ref=f8e45]: Virtual Services
        - list [ref=f8e54]:
          - listitem [ref=f8e56] [cursor=pointer]:
            - generic [ref=f8e57]: Care Team Work List
          - listitem [ref=f8e64] [cursor=pointer]:
            - generic [ref=f8e65]: Enrollments
          - listitem [ref=f8e72] [cursor=pointer]:
            - generic [ref=f8e73]: Patient Assessments
          - generic [ref=f8e79]:
            - listitem [ref=f8e80] [cursor=pointer]:
              - generic [ref=f8e81]: Alerts
            - separator [ref=f8e87]
          - listitem [ref=f8e89] [cursor=pointer]:
            - generic [ref=f8e94]:
              - generic [ref=f8e95]: Tasks
              - generic [ref=f8e96]: "164"
          - generic [ref=f8e97]:
            - listitem [ref=f8e98] [cursor=pointer]:
              - generic [ref=f8e99]: Communications
            - separator [ref=f8e105]
          - generic [ref=f8e106]:
            - listitem [ref=f8e107] [cursor=pointer]:
              - generic [ref=f8e108]: Billing
            - separator [ref=f8e114]
          - generic [ref=f8e115]:
            - listitem [ref=f8e116] [cursor=pointer]:
              - generic [ref=f8e117]: Reports
            - separator [ref=f8e123]
          - listitem [ref=f8e125] [cursor=pointer]:
            - generic [ref=f8e126]: Document Library
          - listitem [ref=f8e133] [cursor=pointer]:
            - generic [ref=f8e134]: CCM Library
          - listitem [ref=f8e141] [cursor=pointer]:
            - generic [ref=f8e142]: PCM Library
          - listitem [ref=f8e149] [cursor=pointer]:
            - generic [ref=f8e150]: RPM Library
          - generic [ref=f8e156]:
            - listitem [ref=f8e157] [cursor=pointer]:
              - generic [ref=f8e158]: RTM Library
            - separator [ref=f8e164]
          - listitem [ref=f8e166] [cursor=pointer]:
            - generic [ref=f8e167]: Training Library
      - generic "Call Center" [ref=f8e174]:
        - listitem [ref=f8e175] [cursor=pointer]:
          - generic [ref=f8e179]: Call Center
      - generic "Revenue Cycle Management" [ref=f8e185]:
        - listitem [ref=f8e186] [cursor=pointer]:
          - generic [ref=f8e190]: Revenue Cycle Management
      - generic "Omni Channel" [ref=f8e196]:
        - listitem [ref=f8e197] [cursor=pointer]:
          - generic [ref=f8e201]: Omni Channel
      - separator [ref=f8e206]
      - listitem [ref=f8e207] [cursor=pointer]:
        - generic [ref=f8e211]: Settings
    - paragraph [ref=f8e215]: Jemes Cory
    - list [ref=f8e217]:
      - listitem [ref=f8e218] [cursor=pointer]:
        - generic [ref=f8e222]: Logout
    - generic "Collapse sidebar":
      - listitem
  - main [ref=f8e223]:
    - generic [ref=f8e225]:
      - group "Platform" [ref=f8e226]:
        - button "RPM" [disabled]
        - button "RTM" [pressed] [ref=f8e227] [cursor=pointer]
        - button "CCM" [disabled]
        - button "PCM" [disabled]
      - generic [ref=f8e228]:
        - generic [ref=f8e235]:
          - generic [ref=f8e236]:
            - generic [ref=f8e237]: Ullrich, Becky
            - generic [ref=f8e238]:
              - text: Male | 02-13-2023 |
              - generic [ref=f8e239]: RTM - Enrolled 08-24-2026
          - generic [ref=f8e240]:
            - generic [ref=f8e241]: User hasn't logged in
            - button [ref=f8e243] [cursor=pointer]
        - generic [ref=f8e248]:
          - generic [ref=f8e249]:
            - paragraph [ref=f8e250]: Upcoming Appointment
            - paragraph [ref=f8e251]: "-"
          - generic [ref=f8e252]:
            - paragraph [ref=f8e253]: Last Appointment
            - paragraph [ref=f8e254]: "-"
        - generic [ref=f8e258]:
          - generic [ref=f8e259]:
            - paragraph [ref=f8e260]: Global Comment
            - button [ref=f8e261] [cursor=pointer]
          - paragraph [ref=f8e266]: Type Your Comment...
        - button "Text Message" [ref=f8e269] [cursor=pointer]
      - generic [ref=f8e275]:
        - tablist [ref=f8e278]:
          - tab "Monitoring" [selected] [ref=f8e279] [cursor=pointer]
          - tab "Vitals" [ref=f8e280] [cursor=pointer]
          - tab "Assessment" [ref=f8e281] [cursor=pointer]
          - tab "Tasks" [ref=f8e282] [cursor=pointer]
          - tab "Documents" [ref=f8e283] [cursor=pointer]
          - tab "Home Exercise" [ref=f8e284] [cursor=pointer]
          - tab "Medical History" [ref=f8e285] [cursor=pointer]
          - tab "Enrollments" [ref=f8e286] [cursor=pointer]
          - tab "Care Team" [ref=f8e287] [cursor=pointer]
          - tab "Training Library" [ref=f8e288] [cursor=pointer]
          - tab "Billing" [ref=f8e289] [cursor=pointer]
          - tab "Summary" [ref=f8e290] [cursor=pointer]
        - generic [ref=f8e292] [cursor=pointer]
      - generic [ref=f8e296]:
        - generic [ref=f8e299]:
          - button "App Chat" [ref=f8e300]:
            - img [ref=f8e302] [cursor=pointer]
          - button "Text Message" [ref=f8e304]:
            - img [ref=f8e306] [cursor=pointer]
          - button "Incoming Text Message" [ref=f8e308]:
            - img [ref=f8e310] [cursor=pointer]
          - combobox "Select" [ref=f8e312]
          - button "Open" [ref=f8e314] [cursor=pointer]
          - group
        - generic [ref=f8e317]:
          - generic [ref=f8e319]:
            - progressbar [ref=f8e323]
            - separator [ref=f8e326]
            - generic [ref=f8e327]:
              - generic [ref=f8e328]:
                - generic [ref=f8e330]:
                  - textbox "Type your message..." [disabled] [ref=f8e331]
                  - group
                - button [ref=f8e332] [cursor=pointer]
                - button [disabled]
                - generic [ref=f8e335]:
                  - button [ref=f8e336] [cursor=pointer]
                  - button [ref=f8e339] [cursor=pointer]
                  - button [ref=f8e343] [cursor=pointer]
                  - paragraph [ref=f8e347]: 00:05:00
              - generic [ref=f8e348]:
                - button "Response Library" [ref=f8e349] [cursor=pointer]
                - button "Escalate to Provider" [ref=f8e354] [cursor=pointer]
                - button "Assign Enrollment" [ref=f8e359] [cursor=pointer]
                - button "Add Note Summary" [ref=f8e364] [cursor=pointer]
                - button "Send" [ref=f8e369] [cursor=pointer]
          - generic [ref=f8e375]:
            - generic [ref=f8e376]:
              - generic [ref=f8e377]: 1/31 Days
              - generic [ref=f8e379]:
                - generic [ref=f8e380]:
                  - generic [ref=f8e383]: 24 Aug - 23 Sep
                  - img [ref=f8e384] [cursor=pointer]
                - progressbar [ref=f8e387]
            - generic [ref=f8e390]:
              - generic [ref=f8e394]:
                - button "Choose date, selected date is Aug 1, 2026" [ref=f8e396] [cursor=pointer]
                - textbox "Select Month" [ref=f8e399]: Aug 2026
                - button "Clear" [ref=f8e401] [cursor=pointer]
                - group
              - generic [ref=f8e404]:
                - paragraph [ref=f8e405]: INTERACTIONS
                - paragraph [ref=f8e406]: "TOTAL TIME: 00:00"
              - generic [ref=f8e408]:
                - progressbar [ref=f8e409]
                - paragraph [ref=f8e412]: "20"
                - paragraph [ref=f8e415]: "40"
                - paragraph [ref=f8e418]: "60"
              - generic [ref=f8e421]:
                - generic [ref=f8e422]:
                  - paragraph [ref=f8e423]: Communication with Patient
                  - generic [ref=f8e424]: 00:00:00
                - generic [ref=f8e425]:
                  - generic [ref=f8e426]: 08/24/2026 08:25 AM
                  - generic [ref=f8e427]:
                    - generic [ref=f8e428] [cursor=pointer]
                    - generic [ref=f8e431] [cursor=pointer]
              - button [ref=f8e434] [cursor=pointer]
        - generic [ref=f8e439]:
          - generic [ref=f8e440]:
            - heading "LATEST READING" [level=5] [ref=f8e441]
            - generic [ref=f8e442]:
              - button [ref=f8e443] [cursor=pointer]
              - button [ref=f8e447] [cursor=pointer]
          - grid [ref=f8e453]:
            - row [ref=f8e454]:
              - columnheader "VITAL NAME" [ref=f8e455]
              - columnheader "DATE" [ref=f8e461]
              - columnheader "LAST UPDATED" [ref=f8e467]
              - columnheader "CURRENT VALUE" [ref=f8e473]
              - columnheader "PREVIOUS VALUE" [ref=f8e479]
              - columnheader "ALERT" [ref=f8e485]
              - columnheader "MONTHLY AVG" [ref=f8e491]
              - columnheader "REVIEW" [ref=f8e497]
              - columnheader "ACTION" [ref=f8e503]
            - rowgroup [ref=f8e509]:
              - row [ref=f8e510]:
                - gridcell "Pain Scale" [ref=f8e511]
                - gridcell "08-24-2026" [ref=f8e512]
                - gridcell "08-24-2026" [ref=f8e513]
                - gridcell "15" [ref=f8e514]
                - gridcell "-" [ref=f8e515]
                - gridcell [ref=f8e516]:
                  - heading "High" [level=6] [ref=f8e518]
                - gridcell "15" [ref=f8e519]
                - gridcell [ref=f8e520]:
                  - checkbox "introduction checkbox" [ref=f8e522] [cursor=pointer]
                - gridcell [ref=f8e525]:
                  - generic [ref=f8e526] [cursor=pointer]
  - button [ref=f8e530] [cursor=pointer]
  - button [ref=f8e534] [cursor=pointer]
```

# Test source

```ts
  65  | 
  66  |         // ────────────────────────────────────────────────────────────
  67  |         // STEP 1 — Add vital on patient chart
  68  |         // ────────────────────────────────────────────────────────────
  69  |         await test.step('Step 1: add Pain Scale on patient chart > RTM > Vitals', async () => {
  70  |             await openPatientRtmTab(page, patientName);
  71  |             await chart.navigateToVitalsTab();
  72  | 
  73  |             // The patient must have an active RTM enrollment for Add Vital
  74  |             // to be enabled. The terminated-patient and activate specs both
  75  |             // leave the seed patient Active — hard-assert here so a regression
  76  |             // upstream surfaces as a real failure rather than a silent skip.
  77  |             const addVitalBtn = page.locator("//button[text()='Add Vital']").first();
  78  |             await addVitalBtn.waitFor({ state: 'attached', timeout: 10000 });
  79  |             await expect(
  80  |                 addVitalBtn,
  81  |                 `${patientName} must have an active RTM enrollment for Add Vital to be enabled`,
  82  |             ).toBeEnabled({ timeout: 10000 });
  83  | 
  84  |             await chart.addVital('Pain Scale', painScaleValue);
  85  |             Logger.info(`Pain Scale = ${painScaleValue} recorded on patient chart`);
  86  |         });
  87  | 
  88  |         // ────────────────────────────────────────────────────────────
  89  |         // STEP 2 — Verify the same vital appears in Latest Reading
  90  |         //           on the chart (sanity check before cross-surface assert)
  91  |         // ────────────────────────────────────────────────────────────
  92  |         await test.step('Step 2: confirm the new reading is in chart > Latest Reading', async () => {
  93  |             // The Latest Reading row for Pain Scale should now show our value.
  94  |             const painScaleRow = page
  95  |                 .locator(`xpath=//*[normalize-space(text())="Pain Scale"]/ancestor::*[self::tr or self::div][1]`)
  96  |                 .first();
  97  |             await expect(painScaleRow).toBeVisible({ timeout: 15000 });
  98  |             await expect(painScaleRow).toContainText(String(painScaleValue), { timeout: 15000 });
  99  |             Logger.info(`Latest Reading on chart shows Pain Scale = ${painScaleValue}`);
  100 |         });
  101 | 
  102 |         // ────────────────────────────────────────────────────────────
  103 |         // STEP 3 — Verify the same data on Care Team Work List
  104 |         // ────────────────────────────────────────────────────────────
  105 |         await test.step('Step 3: confirm patient + reading appear in Care Team Work List > RTM > Monitoring > Data', async () => {
  106 |             await monitoring.navigateToMonitoring();
  107 |             await monitoring.selectProgramTab('RTM');
  108 |             await monitoring.clickMonitoringCategory('Data');
  109 | 
  110 |             // Patient appearing in the Data bucket for today implies the
  111 |             // reading was registered (Data bucket only includes patients
  112 |             // with at least one reading on the selected date).
  113 |             expect(
  114 |                 await monitoring.isPatientInList(patientName),
  115 |                 `${patientName} should appear in the Data bucket after a same-day chart reading`,
  116 |             ).toBe(true);
  117 |             Logger.info(`${patientName} visible in Care Team Work List > RTM > Monitoring > Data`);
  118 |         });
  119 | 
  120 |         // ────────────────────────────────────────────────────────────
  121 |         // STEP 4 — Drill into the patient row and verify the SAME
  122 |         //           vital value appears (true cross-surface sync)
  123 |         // ────────────────────────────────────────────────────────────
  124 |         await test.step('Step 4: open patient readings panel and verify Pain Scale value matches', async () => {
  125 |             // The patient name is clickable in the Data list — clicking it
  126 |             // opens the readings detail panel that lists each vital + value.
  127 |             const patientCell = page.getByText(patientName, { exact: false }).first();
  128 |             await patientCell.waitFor({ state: 'visible', timeout: 10000 });
  129 |             await patientCell.click();
  130 |             await page.waitForLoadState('networkidle').catch(() => { /* noop */ });
  131 | 
  132 |             // The detail panel shows "Pain Scale" alongside the recorded
  133 |             // value. Anchor on a real grid row that has BOTH the vital
  134 |             // name and the value — the previous version used a bare
  135 |             // `//*[contains(., 'Pain Scale') and contains(., '15')].first()`
  136 |             // which matches the OUTERMOST element containing both texts
  137 |             // (typically <body>) because `contains(., …)` traverses
  138 |             // descendants. That would have passed even if the value
  139 |             // weren't in any actual row.
  140 |             const readingMatch = () => page
  141 |                 .getByRole('row')
  142 |                 .filter({ hasText: 'Pain Scale' })
  143 |                 .filter({ hasText: new RegExp(`\\b${painScaleValue}\\b`) })
  144 |                 .first();
  145 |             // The chart→worklist vital sync is an async backend job that can take
  146 |             // 30–90s (longer under parallel load), so a single 20s wait is too
  147 |             // short. Poll with reload until the synced value appears.
  148 |             await expect
  149 |                 .poll(async () => {
  150 |                     if (await readingMatch().isVisible({ timeout: 2500 }).catch(() => false)) return true;
  151 |                     await page.reload();
  152 |                     await page.waitForLoadState('domcontentloaded', { timeout: 15000 }).catch(() => { /* noop */ });
  153 |                     await page.waitForTimeout(2000);
  154 |                     const cell = page.getByText(patientName, { exact: false }).first();
  155 |                     if (await cell.isVisible({ timeout: 3000 }).catch(() => false)) {
  156 |                         await cell.click().catch(() => { /* noop */ });
  157 |                         await page.waitForTimeout(1500);
  158 |                     }
  159 |                     return await readingMatch().isVisible({ timeout: 2500 }).catch(() => false);
  160 |                 }, {
  161 |                     timeout: 90000,
  162 |                     intervals: [5000, 10000, 15000, 20000],
  163 |                     message: `Care Team Work List should show Pain Scale = ${painScaleValue} synced from the chart`,
  164 |                 })
> 165 |                 .toBe(true);
      |                  ^ Error: Care Team Work List should show Pain Scale = 15 synced from the chart
  166 |             Logger.info(`Vitals sync verified: Pain Scale = ${painScaleValue} matches across patient chart and Care Team Work List`);
  167 |         });
  168 |     });
  169 | });
  170 | 
```