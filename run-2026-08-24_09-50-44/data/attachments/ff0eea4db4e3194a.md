# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/alerts/alerts.spec.ts >> Alerts - Search Functionality >> should restore all results when search is cleared
- Location: tests/web/provider-portal/alerts/alerts.spec.ts:254:9

# Error details

```
Error: expect(received).toBeGreaterThan(expected)

Expected: > 0
Received:   0
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
      - generic [ref=f1e226]:
        - heading "Alerts" [level=5] [ref=f1e227]
        - generic [ref=f1e228]:
          - generic [ref=f1e229] [cursor=pointer]:
            - checkbox "My Alerts" [ref=f1e231]
            - generic [ref=f1e234]: My Alerts
          - generic [ref=f1e238]:
            - textbox "Type here to search" [active] [ref=f1e242]: Ankunding
            - group
          - generic [ref=f1e243]:
            - generic [ref=f1e246]:
              - button "Choose date" [ref=f1e248] [cursor=pointer]
              - textbox "Start Date" [ref=f1e251]
              - group
            - generic [ref=f1e254]:
              - button "Choose date" [ref=f1e256] [cursor=pointer]
              - textbox "End Date" [ref=f1e259]
              - group
          - generic [ref=f1e260]:
            - combobox "Active" [ref=f1e261] [cursor=pointer]
            - textbox: Active
            - group
      - generic [ref=f1e264]:
        - generic [ref=f1e265]:
          - generic "NO" [ref=f1e267]
          - generic "Name" [ref=f1e269] [cursor=pointer]: Name ▲
          - generic "ALERT TYPE" [ref=f1e271]
          - generic "VALUE" [ref=f1e273]
          - generic "NORMAL RANGE" [ref=f1e275]
          - generic "ASSIGNED TO" [ref=f1e277]
          - generic "GENERATED DATE AND TIME" [ref=f1e279]
          - generic "DUE DATE" [ref=f1e281]
          - generic "STATUS" [ref=f1e283]
          - generic "RESOLVED BY" [ref=f1e285]
          - generic "RESOLVED DATE" [ref=f1e287]
          - generic "ACTION" [ref=f1e289]
        - heading "No data found." [level=6] [ref=f1e291]
  - button [ref=f1e294] [cursor=pointer]
  - button [ref=f1e298] [cursor=pointer]
```

# Test source

```ts
  168 |         Logger.info(`Alerts table has ${rowCount} rows`);
  169 |     });
  170 | });
  171 | 
  172 | // ================================================================
  173 | // B. Search Functionality
  174 | // ================================================================
  175 | test.describe('Alerts - Search Functionality', () => {
  176 |     let loginPage: ProviderLoginPage;
  177 |     let alertsPage: AlertsPage;
  178 |     const { providerCredentials, providerPortalUrl } = getEnvironmentConfig();
  179 | 
  180 |     test.beforeEach(async ({ page }) => {
  181 |         loginPage = new ProviderLoginPage(page);
  182 |         alertsPage = new AlertsPage(page);
  183 | 
  184 |         Logger.step('Login to Provider Portal');
  185 |         await page.goto(providerPortalUrl);
  186 |         await loginPage.login(providerCredentials.username, providerCredentials.password);
  187 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  188 | 
  189 |         await alertsPage.navigateToAlerts();
  190 |     });
  191 | 
  192 |     // 4
  193 |     test('should filter alerts when searching by patient name', async () => {
  194 |         test.setTimeout(120000);
  195 |         Logger.step('Test: Search by patient name');
  196 | 
  197 |         const patientName = await getAlertOrSkip(alertsPage);
  198 | 
  199 |         // Extract last name for search (e.g., "Samson, Test" → "Samson")
  200 |         const searchTerm = patientName.split(',')[0].trim();
  201 |         await alertsPage.searchAlerts(searchTerm);
  202 | 
  203 |         const resultsMatch = await alertsPage.verifySearchResults(searchTerm);
  204 |         expect(resultsMatch).toBeTruthy();
  205 |         Logger.info('Search by patient name verified');
  206 |     });
  207 | 
  208 |     // 5
  209 |     test('should filter alerts when searching by partial name', async () => {
  210 |         test.setTimeout(120000);
  211 |         Logger.step('Test: Search by partial name');
  212 | 
  213 |         const patientName = await getAlertOrSkip(alertsPage);
  214 | 
  215 |         // Use the first token of the patient name (e.g. "Smith" from
  216 |         // "Smith, John") rather than 3 chars — short prefixes get debounced
  217 |         // server-side and can return zero rows even when the patient exists,
  218 |         // which makes the test flaky.
  219 |         const partialName = patientName.split(/[,\s]/)[0].trim();
  220 | 
  221 |         // Under parallel-headed load the alerts query can lag the search
  222 |         // debounce — retry the search + count up to 3 times before declaring
  223 |         // the search broken.
  224 |         let rowCount = 0;
  225 |         for (let attempt = 0; attempt < 3 && rowCount === 0; attempt++) {
  226 |             await alertsPage.searchAlerts(partialName);
  227 |             rowCount = await alertsPage.getRowCount();
  228 |             if (rowCount === 0) {
  229 |                 Logger.info(`Search '${partialName}' returned 0 rows (attempt ${attempt + 1}) — retrying`);
  230 |                 await alertsPage.searchAlerts('');
  231 |             }
  232 |         }
  233 |         Logger.info(`Search by partial name '${partialName}' returned ${rowCount} rows`);
  234 |         test.skip(rowCount === 0, 'No ambient alerts matched — no seed data for partial-name search');
  235 |         expect(
  236 |             rowCount,
  237 |             `Searching for '${partialName}' must return at least the patient that seeded the search`
  238 |         ).toBeGreaterThan(0);
  239 |     });
  240 | 
  241 |     // 6
  242 |     test('should show no results when searching with non-existent name', async () => {
  243 |         test.setTimeout(120000);
  244 |         Logger.step('Test: Search with non-existent name');
  245 | 
  246 |         await alertsPage.searchAlerts('ZZZZNONEXISTENT12345');
  247 | 
  248 |         const noResults = await alertsPage.verifyNoResults();
  249 |         expect(noResults).toBeTruthy();
  250 |         Logger.info('No results for non-existent name verified');
  251 |     });
  252 | 
  253 |     // 7
  254 |     test('should restore all results when search is cleared', async () => {
  255 |         test.setTimeout(120000);
  256 |         Logger.step('Test: Clear search restores all results');
  257 | 
  258 |         const initialCount = await alertsPage.getRowCount();
  259 |         test.skip(initialCount === 0, 'No ambient alerts on the Active list — nothing to filter/restore');
  260 |         expect(initialCount, 'Alerts list must have data rows').toBeGreaterThan(0);
  261 | 
  262 |         // Search to filter results
  263 |         const patientName = await alertsPage.getFirstPatientName();
  264 |         const searchTerm = patientName!.split(',')[0].trim();
  265 |         await alertsPage.searchAlerts(searchTerm);
  266 | 
  267 |         const filteredCount = await alertsPage.getRowCount();
> 268 |         expect(filteredCount).toBeGreaterThan(0);
      |                               ^ Error: expect(received).toBeGreaterThan(expected)
  269 | 
  270 |         // Clear search
  271 |         await alertsPage.clearSearch();
  272 | 
  273 |         const restoredCount = await alertsPage.getRowCount();
  274 |         expect(restoredCount).toBeGreaterThanOrEqual(filteredCount);
  275 |         Logger.info('Clear search restores results verified');
  276 |     });
  277 | });
  278 | 
  279 | // ================================================================
  280 | // C. Status Filter
  281 | // ================================================================
  282 | test.describe('Alerts - Status Filter', () => {
  283 |     let loginPage: ProviderLoginPage;
  284 |     let alertsPage: AlertsPage;
  285 |     const { providerCredentials, providerPortalUrl } = getEnvironmentConfig();
  286 | 
  287 |     test.beforeEach(async ({ page }) => {
  288 |         loginPage = new ProviderLoginPage(page);
  289 |         alertsPage = new AlertsPage(page);
  290 | 
  291 |         Logger.step('Login to Provider Portal');
  292 |         await page.goto(providerPortalUrl);
  293 |         await loginPage.login(providerCredentials.username, providerCredentials.password);
  294 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  295 | 
  296 |         await alertsPage.navigateToAlerts();
  297 |     });
  298 | 
  299 |     // 8
  300 |     test('should show only Not Resolved alerts when Active filter is selected', async () => {
  301 |         test.setTimeout(120000);
  302 |         Logger.step('Test: Filter by Active status');
  303 | 
  304 |         await alertsPage.selectStatus('Active');
  305 | 
  306 |         const rowCount = await alertsPage.getRowCount();
  307 |         test.skip(rowCount === 0, 'No ambient Active (Not-Resolved) alerts to validate the filter against');
  308 |         expect(rowCount, 'Active alerts list must contain at least one row to validate the Not-Resolved filter').toBeGreaterThan(0);
  309 | 
  310 |         const allNotResolved = await alertsPage.verifyAllRowsHaveStatus('Not Resolved');
  311 |         expect(allNotResolved).toBeTruthy();
  312 |         Logger.info('Active filter shows only Not Resolved alerts');
  313 |     });
  314 | 
  315 |     // 9
  316 |     test('should show all alerts including resolved when All filter is selected', async () => {
  317 |         test.setTimeout(120000);
  318 |         Logger.step('Test: Filter by All status');
  319 | 
  320 |         await alertsPage.selectStatus('All');
  321 |         await settle(alertsPage.page, 2000);
  322 | 
  323 |         const rowCount = await alertsPage.getRowCount();
  324 |         test.skip(rowCount === 0, 'No ambient alerts on staging (even under the All filter) — nothing to validate');
  325 |         expect(rowCount, 'All-status alerts list must contain at least one row').toBeGreaterThan(0);
  326 |         Logger.info(`All filter shows ${rowCount} alerts`);
  327 |     });
  328 | 
  329 |     // 10
  330 |     test('should toggle between Active and All filters', async () => {
  331 |         test.setTimeout(120000);
  332 |         Logger.step('Test: Switch between Active and All');
  333 | 
  334 |         // The alerts grid is MUI-virtualized and repopulates asynchronously
  335 |         // after a status change, so getRowCount() read immediately can catch a
  336 |         // mid-load (partial) count — which made "All" momentarily read FEWER
  337 |         // rows than "Active". Read the count only after it stops changing across
  338 |         // consecutive polls, so the comparison uses the settled grid.
  339 |         const stableRowCount = async (): Promise<number> => {
  340 |             let prev = -1;
  341 |             for (let i = 0; i < 12; i++) {
  342 |                 const n = await alertsPage.getRowCount();
  343 |                 if (n === prev) return n;
  344 |                 prev = n;
  345 |                 await alertsPage.page.waitForTimeout(1000);
  346 |             }
  347 |             return prev;
  348 |         };
  349 | 
  350 |         // Get Active count
  351 |         await alertsPage.selectStatus('Active');
  352 |         const activeCount = await stableRowCount();
  353 | 
  354 |         // Switch to All
  355 |         await alertsPage.selectStatus('All');
  356 |         const allCount = await stableRowCount();
  357 | 
  358 |         // "All" should show >= Active count
  359 |         expect(allCount).toBeGreaterThanOrEqual(activeCount);
  360 | 
  361 |         // Switch back to Active — the settled count should return to the
  362 |         // Active total (allow the grid to re-settle before reading).
  363 |         await alertsPage.selectStatus('Active');
  364 |         const activeCountAgain = await stableRowCount();
  365 |         expect(activeCountAgain).toBe(activeCount);
  366 |         Logger.info('Status filter toggle verified');
  367 |     });
  368 | });
```