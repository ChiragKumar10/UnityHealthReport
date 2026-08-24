# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/enrollment/Add-Enrollments.spec.ts >> Provider Portal - Add Enrollment Tests >> Add Enrollment — patient enrolls as New then moves to Active
- Location: tests/web/provider-portal/enrollment/Add-Enrollments.spec.ts:76:7

# Error details

```
Error: Patient "Doyle" (RTM) should appear in the Active section after Move to Active

expect(locator).toBeVisible() failed

Locator: locator('//div[contains(@class,"css-1hhl13x")] | //div[(./div[normalize-space()="RPM"] or ./div[normalize-space()="RTM"] or ./div[normalize-space()="CCM"] or ./div[normalize-space()="PCM"]) and count(./div) >= 6]').filter({ hasText: 'Doyle' }).filter({ hasText: 'RTM' }).first()
Expected: visible
Timeout: 30000ms
Error: element(s) not found

Call log:
  - Patient "Doyle" (RTM) should appear in the Active section after Move to Active with timeout 30000ms
  - waiting for locator('//div[contains(@class,"css-1hhl13x")] | //div[(./div[normalize-space()="RPM"] or ./div[normalize-space()="RTM"] or ./div[normalize-space()="CCM"] or ./div[normalize-space()="PCM"]) and count(./div) >= 6]').filter({ hasText: 'Doyle' }).filter({ hasText: 'RTM' }).first()

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
  - heading "Enrollments" [level=6]
  - button "Choose date, selected date is Aug 24, 2026"
  - textbox "Start Date": 08-24-2026
  - button "Clear"
  - button "Choose date, selected date is Aug 24, 2026"
  - textbox "End Date": 08-24-2026
  - button "Clear"
  - combobox "Remote Therapeutic Monitoring (RTM)"
  - combobox "Active"
  - button "Add Enrollment"
  - text: SR NO NAME ▲ PROGRAM ENROLLED DATE STATUS DIAGNOSIS CODES(ICD) CARE MANAGER PROVIDER LOCATION ACTION 01 Dibbert, Carson RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +2 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 02 Oberbrunner, Vito RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 03 Murazik, Kiera RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 04 Champlin, Maryam RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 05 Ullrich, Becky RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 06 Ortiz, Bethany RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 07 Franecki, Ted RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 08 Wilkinson, Burley RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 09 Dibbert, Sedrick RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 10 Veum, Oliver RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 11 Franey, Dorothy RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 12 Johnson, Gwen RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 13 Dickinson, Dejon RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 14 Medhurst, Darlene RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 15 Lakin, Grace RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation 16 Mann, Ivah RTM 08-24-2026
  - heading "active" [level=6]
  - text: A111-Test ... +1 Autofirstarnnuw Autolastarnnuw Anny Vate Automation
- button
- button
```

# Test source

```ts
  32  | 
  33  |     await enrollment.addEnrolmentBtn.click();
  34  |     await enrollment.patientDrodown.waitFor({ state: 'visible', timeout: 15000 });
  35  | 
  36  |     // Select our seeded (un-enrolled) patient deterministically — no letter-guessing.
  37  |     // Retry to tolerate global-search indexing lag for a just-created patient
  38  |     // (worse under concurrent load).
  39  |     const patientOption = page.locator('//ul[@role="listbox"]//li')
  40  |       .filter({ hasText: seededPatient.lastName })
  41  |       .first();
  42  |     let optVisible = false;
  43  |     for (let attempt = 0; attempt < 6 && !optVisible; attempt++) {
  44  |       await enrollment.patientDrodown.click();
  45  |       await enrollment.patientDrodown.fill('');
  46  |       await enrollment.patientDrodown.fill(seededPatient.lastName);
  47  |       optVisible = await patientOption.waitFor({ state: 'visible', timeout: 5000 }).then(() => true).catch(() => false);
  48  |       if (!optVisible) await page.waitForTimeout(2500);
  49  |     }
  50  |     expect(optVisible, `Seeded patient "${seededPatient.lastName}" should appear in the patient dropdown`).toBe(true);
  51  |     await patientOption.click();
  52  | 
  53  |     await enrollment.serviceDropdown.click();
  54  |     await page.locator('//ul[@role="listbox"]//li').first().click();
  55  | 
  56  |     await enrollment.providerDropdown.click();
  57  |     await page.locator('//ul[@role="listbox"]//li').first().click();
  58  | 
  59  |     await enrollment.careMangerDropdown.click();
  60  |     await page.locator('//ul[@role="listbox"]//li').first().click();
  61  | 
  62  |     await enrollment.conditionsDropdown.click();
  63  |     const diagnosisOptions = page.locator('//ul[@role="listbox"]//li');
  64  |     await diagnosisOptions.first().waitFor({ state: 'visible', timeout: 8000 });
  65  |     await diagnosisOptions.first().locator('input').click();
  66  |     await diagnosisOptions.nth(1).locator('input').click();
  67  |     await page.keyboard.press('Escape');
  68  | 
  69  |     await page.locator('//button[contains(., "Cancel")]').click();
  70  | 
  71  |     await expect(page.locator('//h6[text()="New Enrollment"]')).not.toBeVisible();
  72  |     await expect(enrollment.enrollmentListContainer).toBeVisible();
  73  |     Logger.info('Cancel button verified — form closed and navigated back to Enrollment List');
  74  |   });
  75  | 
  76  |   test('Add Enrollment — patient enrolls as New then moves to Active', async ({ page, createSeededPatient }) => {
  77  |     // 300s: one login + UI patient creation + enroll + New→Active move + two
  78  |     // list verifications, all in a single session on a sluggish staging window.
  79  |     test.setTimeout(300000);
  80  | 
  81  |     const loginPage = new ProviderLoginPage(page);
  82  |     const enrollment = new ProviderEnrollmentsPage(page);
  83  |     const patientManagement = new PatientManagementPage(page);
  84  | 
  85  |     Logger.step('Test: Enroll the seeded patient, verify New, then move to Active');
  86  |     // ONE login, then create the patient in the SAME session (no second login).
  87  |     await loginPage.login(providerCredentials.username, providerCredentials.password);
  88  |     const seededPatient = await createSeededPatient();
  89  |     await enrollment.gotoEnrollmentSection();
  90  | 
  91  |     // Enroll in a RANDOMLY chosen program each run (not always the same one), so
  92  |     // the suite exercises RPM/RTM/CCM/PCM over time. The seeded patient is brand
  93  |     // new with no existing enrollment, so addEnrollment selects it directly.
  94  |     const programsFull = [
  95  |       'Remote Patient Monitoring (RPM)',
  96  |       'Remote Therapeutic Monitoring (RTM)',
  97  |       'Chronic Care Management (CCM)',
  98  |       'Principal Care Management (PCM)',
  99  |     ];
  100 |     const programFull = programsFull[Math.floor(Math.random() * programsFull.length)];
  101 |     const programShort = programFull.match(/\(([^)]+)\)/)?.[1] ?? programFull;
  102 | 
  103 |     const enrollmentData: EnrollmentData = await enrollment.addEnrollment(
  104 |       seededPatient.displayName,
  105 |       programFull,
  106 |       patientManagement,
  107 |     );
  108 |     Logger.info(`Enrolled "${enrollmentData.patientName}" in ${enrollmentData.program}`);
  109 | 
  110 |     // ── Verify the patient appears in the NEW section of the Enrollment List ──
  111 |     await enrollment.gotoEnrollmentSection();
  112 |     await enrollment.applyStatusFilter('New');
  113 |     await enrollment.applyProgramFilter(programFull).catch(() => {});
  114 |     await enrollment.setDateFilterToToday(); // list defaults to a past range; pin to today
  115 |     await expect(
  116 |       enrollment.getEnrollmentRow(seededPatient.lastName, programShort),
  117 |       `Enrolled patient "${seededPatient.lastName}" (${programShort}) should appear in the New section`,
  118 |     ).toBeVisible({ timeout: 30000 });
  119 |     Logger.info(`Verified "${seededPatient.lastName}" is in the New section (${programShort})`);
  120 | 
  121 |     // ── Move the enrollment New → Active ──
  122 |     await enrollment.moveEnrollmentToActive(seededPatient.lastName, programShort);
  123 | 
  124 |     // ── Verify the patient now appears in the ACTIVE section ──
  125 |     await enrollment.gotoEnrollmentSection();
  126 |     await enrollment.applyStatusFilter('Active');
  127 |     await enrollment.applyProgramFilter(programFull).catch(() => {});
  128 |     await enrollment.setDateFilterToToday(); // list defaults to a past range; pin to today
  129 |     await expect(
  130 |       enrollment.getEnrollmentRow(seededPatient.lastName, programShort),
  131 |       `Patient "${seededPatient.lastName}" (${programShort}) should appear in the Active section after Move to Active`,
> 132 |     ).toBeVisible({ timeout: 30000 });
      |       ^ Error: Patient "Doyle" (RTM) should appear in the Active section after Move to Active
  133 |     Logger.info(`Verified "${seededPatient.lastName}" moved to the Active section (${programShort})`);
  134 |   });
  135 | });
  136 | 
```