# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/monitoring/billing-enrollments-paid-status-workflow.spec.ts >> Billing > Enrollments — paid-status workflow >> update paid status E2E — clicking Update + marking as "Paid" flips row and surfaces success toast
- Location: tests/web/provider-portal/monitoring/billing-enrollments-paid-status-workflow.spec.ts:155:13

# Error details

```
TimeoutError: locator.waitFor: Timeout 10000ms exceeded.
Call log:
  - waiting for locator('//*[normalize-space(text())="Primary Role" or normalize-space(text())="Primary Role *"]/following::*[(@role="combobox" or @role="button" or self::div[contains(@class,"MuiSelect")])][1]').first() to be visible

```

# Page snapshot

```yaml
- generic [ref=f1e1]:
  - generic [ref=f1e4]:
    - banner [ref=f1e5]:
      - generic [ref=f1e10]:
        - generic [ref=f1e13]:
          - combobox [ref=f1e17]
          - button [ref=f1e19] [cursor=pointer]
          - group
        - button [ref=f1e22] [cursor=pointer]:
          - paragraph [ref=f1e25]: New Patient
        - generic [ref=f1e26]:
          - button [ref=f1e27] [cursor=pointer]
          - button [ref=f1e31] [cursor=pointer]
    - generic [ref=f1e36]:
      - list [ref=f1e38]:
        - generic [ref=f1e39]:
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
        - listitem [ref=f1e175] [cursor=pointer]:
          - generic [ref=f1e179]: Call Center
        - listitem [ref=f1e186] [cursor=pointer]:
          - generic [ref=f1e190]: Revenue Cycle Management
        - listitem [ref=f1e197] [cursor=pointer]:
          - generic [ref=f1e201]: Omni Channel
        - separator [ref=f1e206]
        - listitem [ref=f1e207] [cursor=pointer]:
          - generic [ref=f1e211]: Settings
      - paragraph [ref=f1e215]: Jemes Cory
      - list [ref=f1e217]:
        - listitem [ref=f1e218] [cursor=pointer]:
          - generic [ref=f1e222]: Logout
      - generic:
        - listitem
    - main [ref=f1e223]:
      - generic [ref=f1e225]:
        - generic [ref=f1e227]:
          - tablist [ref=f1e232]:
            - tab [selected] [ref=f1e233] [cursor=pointer]: Profile
            - tab [ref=f1e234] [cursor=pointer]: Unity Users
            - tab [ref=f1e235] [cursor=pointer]: Insurance
            - tab [ref=f1e236] [cursor=pointer]: Location
            - tab [ref=f1e237] [cursor=pointer]: Procedure Codes
            - tab [ref=f1e238] [cursor=pointer]: Tickets
            - tab [ref=f1e239] [cursor=pointer]: FAQ
          - generic [ref=f1e241]:
            - button [ref=f1e242] [cursor=pointer]: Update Password
            - button [ref=f1e245] [cursor=pointer]: Edit Profile
        - generic [ref=f1e250]:
          - generic [ref=f1e256]:
            - generic [ref=f1e257]:
              - heading [level=6] [ref=f1e258]: Name
              - paragraph [ref=f1e259]: Jemes Cory
            - generic [ref=f1e260]:
              - heading [level=6] [ref=f1e261]: Username
              - paragraph [ref=f1e262]: jemes
            - generic [ref=f1e263]:
              - heading [level=6] [ref=f1e264]: Email
              - paragraph [ref=f1e265]: jemes@mailinator.com
            - generic [ref=f1e266]:
              - heading [level=6] [ref=f1e267]: Role
              - paragraph [ref=f1e268]: Practice Admin > Billing Admin, Call Center, Omni Channel
          - generic [ref=f1e270]:
            - heading [level=6] [ref=f1e272]: Bio
            - heading [level=6] [ref=f1e274]: N/A
  - generic [ref=f1e280]:
    - generic [ref=f1e281]:
      - heading "EDIT UNITY USER" [level=6] [ref=f1e282]
      - generic [ref=f1e284]:
        - button [ref=f1e285] [cursor=pointer]:
          - heading "Cancel" [level=6] [ref=f1e286]
        - button [ref=f1e287] [cursor=pointer]:
          - heading "Save" [level=6] [ref=f1e288]
    - generic [ref=f1e289]:
      - generic [ref=f1e290]:
        - heading "First Name*" [level=6] [ref=f1e292]
        - textbox "First Name" [ref=f1e294]: Jemes
      - generic [ref=f1e295]:
        - heading "Last Name*" [level=6] [ref=f1e297]
        - textbox "Last Name" [ref=f1e299]: Cory
    - generic [ref=f1e300]:
      - generic [ref=f1e301]:
        - heading "Username*" [level=6] [ref=f1e303]
        - textbox "Username" [ref=f1e305]: jemes
      - generic [ref=f1e306]:
        - heading "Password" [level=6] [ref=f1e308]
        - textbox "Password" [ref=f1e310]
      - generic [ref=f1e311]:
        - heading "Email" [level=6] [ref=f1e313]
        - textbox "Enter Email" [ref=f1e315]: jemes@mailinator.com
    - generic [ref=f1e316]:
      - heading "Application Access & Roles*" [level=6] [ref=f1e318]
      - generic [ref=f1e319]:
        - generic [ref=f1e320]:
          - checkbox [checked] [ref=f1e322] [cursor=pointer]
          - heading "Virtual Services" [level=6] [ref=f1e325]
          - generic [ref=f1e326]:
            - generic:
              - checkbox [checked] [disabled]
            - heading "Default" [level=6] [ref=f1e327]
        - generic [ref=f1e328]:
          - button "Billing" [ref=f1e329] [cursor=pointer]
          - button "Care coordinator" [ref=f1e331] [cursor=pointer]
          - button "Care Team" [ref=f1e333] [cursor=pointer]
          - button "Practice Admin" [ref=f1e335] [cursor=pointer]
          - button "Provider" [ref=f1e337] [cursor=pointer]
          - button "Support staff" [ref=f1e339] [cursor=pointer]
          - button "UH Admin" [ref=f1e341] [cursor=pointer]
      - generic [ref=f1e343]:
        - generic [ref=f1e344]:
          - checkbox [checked] [ref=f1e346] [cursor=pointer]
          - heading "Call Center" [level=6] [ref=f1e349]
          - generic [ref=f1e350]:
            - checkbox [ref=f1e352] [cursor=pointer]
            - heading "Default" [level=6] [ref=f1e355]
        - generic [ref=f1e356]:
          - button "Call Center Agent" [ref=f1e357] [cursor=pointer]
          - button "Admin" [ref=f1e359] [cursor=pointer]
          - button "Support staff" [ref=f1e361] [cursor=pointer]
          - button "UH Admin" [ref=f1e363] [cursor=pointer]
        - generic [ref=f1e365]:
          - generic [ref=f1e366] [cursor=pointer]:
            - checkbox "Calls" [checked] [ref=f1e368]
            - generic [ref=f1e371]: Calls
          - generic [ref=f1e372] [cursor=pointer]:
            - checkbox "Voicemail" [checked] [ref=f1e374]
            - generic [ref=f1e377]: Voicemail
          - generic [ref=f1e378] [cursor=pointer]:
            - checkbox "SMS" [checked] [ref=f1e380]
            - generic [ref=f1e383]: SMS
      - generic [ref=f1e384]:
        - generic [ref=f1e385]:
          - checkbox [checked] [ref=f1e387] [cursor=pointer]
          - heading "Revenue Cycle Management" [level=6] [ref=f1e390]
          - generic [ref=f1e391]:
            - checkbox [ref=f1e393] [cursor=pointer]
            - heading "Default" [level=6] [ref=f1e396]
        - generic [ref=f1e397]:
          - button "Billing Admin" [ref=f1e398] [cursor=pointer]
          - button "Admin" [ref=f1e400] [cursor=pointer]
          - button "Support staff" [ref=f1e402] [cursor=pointer]
          - button "UH Admin" [ref=f1e404] [cursor=pointer]
      - generic [ref=f1e406]:
        - generic [ref=f1e407]:
          - checkbox [checked] [ref=f1e409] [cursor=pointer]
          - heading "Omni Channel" [level=6] [ref=f1e412]
          - generic [ref=f1e413]:
            - checkbox [ref=f1e415] [cursor=pointer]
            - heading "Default" [level=6] [ref=f1e418]
        - generic [ref=f1e419]:
          - button "Omni Agent" [ref=f1e420] [cursor=pointer]
          - button "Admin" [ref=f1e422] [cursor=pointer]
          - button "Support staff" [ref=f1e424] [cursor=pointer]
          - button "UH Admin" [ref=f1e426] [cursor=pointer]
    - generic [ref=f1e428]:
      - generic [ref=f1e429]: Profile Photo
      - generic [ref=f1e432] [cursor=pointer]:
        - heading "Drop Here Image" [level=6] [ref=f1e435]
        - heading "No File Selected" [level=6] [ref=f1e439]
    - generic [ref=f1e440]:
      - heading "Bio" [level=6] [ref=f1e442]
      - textbox "Enter Bio" [ref=f1e444]
```

# Test source

```ts
  1  | import { Page, expect } from '@playwright/test';
  2  | import { settle } from './wait-helpers';
  3  | import { Logger } from './logger';
  4  | 
  5  | /**
  6  |  * Verifies (or sets) the logged-in provider's Primary Role to
  7  |  * "Billing Admin" via Sidebar > Settings > Edit Profile.
  8  |  *
  9  |  * Idempotent: if the user already holds Billing Admin we click
  10 |  * Cancel and return. Otherwise we open the Primary Role dropdown,
  11 |  * pick Billing Admin, and Save.
  12 |  *
  13 |  * The ACTION column on Billing > Enrollments and the Update drawer
  14 |  * are gated on this role — call this helper in the `beforeEach` of
  15 |  * any workflow spec that exercises the Claim/Update flows.
  16 |  */
  17 | export async function ensureBillingAdminRole(page: Page): Promise<void> {
  18 |     Logger.step('Verify / set profile role to "Billing Admin"');
  19 | 
  20 |     const settingsNav = page.locator('li', { hasText: /^Settings$/ }).first();
  21 |     await settingsNav.waitFor({ state: 'visible', timeout: 15000 });
  22 |     await settingsNav.click();
  23 |     await page.waitForLoadState('networkidle').catch(() => { /* noop */ });
  24 | 
  25 |     const editProfile = page.getByText(/Edit Profile/i, { exact: false }).first();
  26 |     await editProfile.waitFor({ state: 'visible', timeout: 15000 });
  27 |     await editProfile.click();
  28 | 
  29 |     await expect(
  30 |         page.getByRole('heading', { name: /EDIT UNITY USER/i }).first(),
  31 |         'EDIT UNITY USER drawer must open',
  32 |     ).toBeVisible({ timeout: 15000 });
  33 | 
  34 |     // If "Billing Admin" text appears anywhere following the
  35 |     // "Primary Role" label inside the drawer, the role is already set.
  36 |     const billingAdminValue = page
  37 |         .locator(
  38 |             'xpath=//*[normalize-space(text())="Primary Role" or normalize-space(text())="Primary Role *"]/following::*[normalize-space(text())="Billing Admin"][1]',
  39 |         )
  40 |         .first();
  41 |     const alreadyBillingAdmin = await billingAdminValue.isVisible({ timeout: 5000 }).catch(() => false);
  42 | 
  43 |     if (alreadyBillingAdmin) {
  44 |         Logger.info('Primary Role is already "Billing Admin" — closing drawer without changes');
  45 |         const cancelBtn = page.getByRole('button', { name: /^Cancel$/i }).first();
  46 |         await cancelBtn.click();
  47 |         await page
  48 |             .getByRole('heading', { name: /EDIT UNITY USER/i })
  49 |             .first()
  50 |             .waitFor({ state: 'hidden', timeout: 10000 })
  51 |             .catch(() => { /* noop */ });
  52 |         return;
  53 |     }
  54 | 
  55 |     Logger.step('Primary Role is NOT Billing Admin — updating');
  56 |     const primaryRoleSelect = page
  57 |         .locator(
  58 |             'xpath=//*[normalize-space(text())="Primary Role" or normalize-space(text())="Primary Role *"]/following::*[(@role="combobox" or @role="button" or self::div[contains(@class,"MuiSelect")])][1]',
  59 |         )
  60 |         .first();
> 61 |     await primaryRoleSelect.waitFor({ state: 'visible', timeout: 10000 });
     |                             ^ TimeoutError: locator.waitFor: Timeout 10000ms exceeded.
  62 |     await primaryRoleSelect.click();
  63 | 
  64 |     await page.getByRole('option').first().waitFor({ state: 'visible', timeout: 10000 });
  65 |     await page.getByRole('option', { name: /Billing\s*Admin/i }).first().click();
  66 |     await settle(page, 500);
  67 | 
  68 |     const saveBtn = page.getByRole('button', { name: /^Save$/i }).first();
  69 |     await saveBtn.click();
  70 |     await page.waitForLoadState('networkidle').catch(() => { /* noop */ });
  71 |     Logger.info('Primary Role saved as "Billing Admin"');
  72 | }
  73 | 
```