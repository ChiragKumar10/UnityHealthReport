# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/settings/unity-users.spec.ts >> Settings - Unity Users Tab >> should prevent deleted provider from logging in
- Location: tests/web/provider-portal/settings/unity-users.spec.ts:699:9

# Error details

```
TimeoutError: page.waitForSelector: Timeout 10000ms exceeded.
Call log:
  - waiting for locator('//input[@name="userName"]') to be visible

```

# Test source

```ts
  875  |                 .filter((e) => getComputedStyle(e as HTMLElement).cursor === 'pointer')
  876  |                 .map((e) => (e.textContent || '').trim())
  877  |                 .filter((t) => t.length > 1 && /[A-Za-z]\s+[A-Za-z]/.test(t)),
  878  |         );
  879  |         Logger.info(`Found ${names.length} user names in list`);
  880  |         return names;
  881  |     }
  882  | 
  883  |     // =============================================
  884  |     // PAGINATION
  885  |     // =============================================
  886  | 
  887  |     async getVisibleRowCount(): Promise<number> {
  888  |         Logger.step('Getting visible row count');
  889  |         await this.page.waitForTimeout(1000);
  890  |         // Count rows in the main list area
  891  |         const rows = this.page.locator('//main//tbody//tr | //main//*[contains(@class,"MuiTypography-title2")]');
  892  |         const count = await rows.count();
  893  |         Logger.info(`Visible row count: ${count}`);
  894  |         return count;
  895  |     }
  896  | 
  897  |     async isPaginationVisible(): Promise<boolean> {
  898  |         Logger.step('Checking if pagination controls are visible');
  899  |         const pagination = this.page.locator(
  900  |             '//*[contains(@class,"MuiTablePagination")] | //*[contains(@class,"pagination")] | //*[contains(text(),"Rows per page")] | //*[contains(text(),"of ")] | //button[@aria-label="Go to next page"] | //button[@aria-label="Go to previous page"]'
  901  |         ).first();
  902  |         const visible = await pagination.isVisible().catch(() => false);
  903  |         Logger.info(`Pagination visible: ${visible}`);
  904  |         return visible;
  905  |     }
  906  | 
  907  |     async clickNextPage(): Promise<void> {
  908  |         Logger.step('Clicking next page button');
  909  |         const nextBtn = this.page.locator(
  910  |             '//button[@aria-label="Go to next page"] | //*[contains(@class,"MuiTablePagination")]//button[last()] | //*[contains(@class,"next")]'
  911  |         ).first();
  912  |         await nextBtn.waitFor({ state: 'visible', timeout: 10000 });
  913  |         await nextBtn.click();
  914  |         await this.page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  915  |         await this.page.waitForTimeout(1000);
  916  |         Logger.info('Next page clicked');
  917  |     }
  918  | 
  919  |     async clickPreviousPage(): Promise<void> {
  920  |         Logger.step('Clicking previous page button');
  921  |         const prevBtn = this.page.locator(
  922  |             '//button[@aria-label="Go to previous page"] | //*[contains(@class,"MuiTablePagination")]//button[1] | //*[contains(@class,"prev")]'
  923  |         ).first();
  924  |         await prevBtn.waitFor({ state: 'visible', timeout: 10000 });
  925  |         await prevBtn.click();
  926  |         await this.page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  927  |         await this.page.waitForTimeout(1000);
  928  |         Logger.info('Previous page clicked');
  929  |     }
  930  | 
  931  |     async getPaginationText(): Promise<string> {
  932  |         Logger.step('Getting pagination text');
  933  |         const paginationText = this.page.locator(
  934  |             '//*[contains(@class,"MuiTablePagination-displayedRows")] | //*[contains(text(),"of ")] | //*[contains(@class,"pagination")]//*[contains(text(),"-")]'
  935  |         ).first();
  936  |         const text = await paginationText.textContent().catch(() => '');
  937  |         Logger.info(`Pagination text: ${text}`);
  938  |         return text || '';
  939  |     }
  940  | 
  941  |     // =============================================
  942  |     // TOTAL PROVIDER COUNT
  943  |     // =============================================
  944  | 
  945  |     async getTotalProviderCount(): Promise<string> {
  946  |         Logger.step('Getting total provider count');
  947  |         // Look for count display — often near the top of the list like "Total: 25" or "25 Users"
  948  |         const countElement = this.page.locator(
  949  |             '//*[contains(text(),"Total")] | //*[contains(text(),"total")] | //*[contains(text(),"Users")] | //*[contains(text(),"users")] | //*[contains(text(),"Providers")] | //*[contains(text(),"providers")] | //*[contains(text(),"Results")] | //*[contains(text(),"results")]'
  950  |         ).first();
  951  |         const visible = await countElement.isVisible().catch(() => false);
  952  |         if (visible) {
  953  |             const text = (await countElement.textContent()) || '';
  954  |             Logger.info(`Total provider count text: ${text.trim()}`);
  955  |             return text.trim();
  956  |         }
  957  |         // Fallback: check pagination text for total
  958  |         const paginationText = await this.getPaginationText();
  959  |         Logger.info(`Provider count from pagination: ${paginationText}`);
  960  |         return paginationText;
  961  |     }
  962  | 
  963  |     // =============================================
  964  |     // LOGIN ATTEMPT (for restriction tests)
  965  |     // =============================================
  966  | 
  967  |     async attemptLoginInNewContext(browser: any, url: string, username: string, password: string): Promise<{ success: boolean; errorMessage: string }> {
  968  |         Logger.step(`Attempting login with username: ${username}`);
  969  |         const newPage = await browser.newPage();
  970  |         try {
  971  |             await newPage.goto(url);
  972  |             await newPage.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  973  | 
  974  |             // Fill login form
> 975  |             await newPage.waitForSelector('//input[@name="userName"]', { state: 'visible', timeout: 10000 });
       |                           ^ TimeoutError: page.waitForSelector: Timeout 10000ms exceeded.
  976  |             await newPage.fill('//input[@name="userName"]', username);
  977  |             await newPage.fill('//input[@type="password"]', password);
  978  |             await newPage.click('//button[@type="submit"]');
  979  |             await newPage.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  980  |             await newPage.waitForTimeout(3000);
  981  | 
  982  |             // Check if login succeeded (redirected to worklist) or failed (still on login/error shown)
  983  |             const currentUrl = newPage.url();
  984  |             const isOnWorkList = currentUrl.includes('/worklist') || currentUrl.includes('/dashboard');
  985  | 
  986  |             if (isOnWorkList) {
  987  |                 Logger.info('Login succeeded — user reached worklist');
  988  |                 return { success: true, errorMessage: '' };
  989  |             }
  990  | 
  991  |             // Check for error message
  992  |             const errorLocator = newPage.locator('//div[contains(@class, "MuiAlert-message")] | //div[contains(@class, "error-message")] | //*[contains(@class,"MuiFormHelperText")] | //*[contains(text(),"Invalid")] | //*[contains(text(),"inactive")] | //*[contains(text(),"disabled")] | //*[contains(text(),"not found")]');
  993  |             const errorVisible = await errorLocator.first().isVisible().catch(() => false);
  994  |             let errorText = '';
  995  |             if (errorVisible) {
  996  |                 errorText = (await errorLocator.first().textContent()) || '';
  997  |             }
  998  | 
  999  |             Logger.info(`Login failed — error: ${errorText || 'No error text found'}`);
  1000 |             return { success: false, errorMessage: errorText };
  1001 |         } finally {
  1002 |             await newPage.close();
  1003 |         }
  1004 |     }
  1005 | }
  1006 | 
```