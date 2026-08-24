# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/documents/documents-full-workflow.spec.ts >> Document - Count Update on Assign >> AUT_DOC_019 - Verify document count increases after upload and assignment
- Location: tests/web/provider-portal/documents/documents-full-workflow.spec.ts:526:9

# Error details

```
Error: Assigned document should appear in patient charting

expect(locator).toContainText(expected) failed

Locator: locator('main')
Expected substring: "CountDoc 1787560460937"
Received string:    "RPMRTMCCMPCMFlatley, LisaMale | 08-17-2023 |CCM - Enrolled 08-24-2026User hasn't logged inProfileUpcoming Appointment-Last Appointment-Global CommentNewType Your Comment...Text MessageChatsCare PlanAssessmentTasksDocumentsHome ExerciseMedical HistoryEnrollmentsCare TeamTraining LibraryBillingSummaryShow Archived​​Assign DocumentAdd DocumentHome›EducationNOFILE NAMETAGSHAREDTYPEMODIFIEDMODIFIED BYACTIONNo data found."
Timeout: 15000ms

Call log:
  - Assigned document should appear in patient charting with timeout 15000ms
  - waiting for locator('main')
    2 × locator resolved to <main class="MuiBox-root css-5hqkkr">…</main>
      - unexpected value "RPMRTMCCMPCMFlatley, LisaMale | 08-17-2023 |CCM - Enrolled 08-24-2026User hasn't logged inProfileUpcoming Appointment-Last Appointment-Global CommentNewType Your Comment...Text MessageChatsCare PlanAssessmentTasksDocumentsHome ExerciseMedical HistoryEnrollmentsCare TeamTraining LibraryBillingSummaryShow Archived​​Assign DocumentAdd DocumentHome›EducationNOFILE NAMETAGSHAREDTYPEMODIFIEDMODIFIED BYACTIONLoading..."
    30 × locator resolved to <main class="MuiBox-root css-5hqkkr">…</main>
       - unexpected value "RPMRTMCCMPCMFlatley, LisaMale | 08-17-2023 |CCM - Enrolled 08-24-2026User hasn't logged inProfileUpcoming Appointment-Last Appointment-Global CommentNewType Your Comment...Text MessageChatsCare PlanAssessmentTasksDocumentsHome ExerciseMedical HistoryEnrollmentsCare TeamTraining LibraryBillingSummaryShow Archived​​Assign DocumentAdd DocumentHome›EducationNOFILE NAMETAGSHAREDTYPEMODIFIEDMODIFIED BYACTIONNo data found."

```

```yaml
- main:
  - group "Platform":
    - button "RPM" [disabled]
    - button "RTM" [disabled]
    - button "CCM" [pressed]
    - button "PCM" [disabled]
  - text: Flatley, Lisa Male | 08-17-2023 | CCM - Enrolled 08-24-2026 User hasn't logged in
  - button "Profile"
  - paragraph: Upcoming Appointment
  - paragraph: "-"
  - paragraph: Last Appointment
  - paragraph: "-"
  - paragraph: Global Comment
  - button "New"
  - paragraph: Type Your Comment...
  - button "Text Message"
  - tablist:
    - tab "Chats"
    - tab "Care Plan"
    - tab "Assessment"
    - tab "Tasks"
    - tab "Documents" [selected]
    - tab "Home Exercise"
    - tab "Medical History"
    - tab "Enrollments"
    - tab "Care Team"
    - tab "Training Library"
    - tab "Billing"
    - tab "Summary"
  - checkbox "Show Archived"
  - text: Show Archived
  - textbox "Type here to search"
  - button "Assign Document"
  - button "Add Document"
  - navigation "breadcrumb":
    - list:
      - listitem:
        - heading "Home" [level=6]
      - listitem:
        - heading "Education" [level=6]
  - text: NO FILE NAME TAG SHARED TYPE MODIFIED MODIFIED BY ACTION
  - heading "No data found." [level=6]
```

# Test source

```ts
  476 |             await page.reload({ waitUntil: 'domcontentloaded' });
  477 |             await page.locator("(//*[contains(text(),'Document Library')])[1]").first().click();
  478 |             await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  479 |             await settle(page, 1500);
  480 |             await docPage.clickFolder('Education');
  481 |             await settle(page, 2500);
  482 | 
  483 |             // Ensure Show Archived is unchecked
  484 |             const archiveCheckbox = page.locator("//input[@type='checkbox']").first();
  485 |             if (await archiveCheckbox.isChecked().catch(() => false)) {
  486 |                 await docPage.toggleShowArchived();
  487 |                 await settle(page, 2000);
  488 |             }
  489 | 
  490 |             // Re-search up to 3 times — the unarchived row can lag a few seconds
  491 |             // behind the server response before appearing in the unfiltered list.
  492 |             let restored = false;
  493 |             for (let attempt = 0; attempt < 3 && !restored; attempt++) {
  494 |                 await docPage.searchDocument(fn);
  495 |                 await settle(page, 1500);
  496 |                 restored = await docPage.isDocumentInList(fn);
  497 |                 if (!restored) await settle(page, 2000);
  498 |             }
  499 |             expect(restored, 'Unarchived document should be visible again').toBeTruthy();
  500 |             Logger.info('Step 7 ✓: Document restored and visible');
  501 |         } else {
  502 |             await page.keyboard.press('Escape');
  503 |             Logger.info('Step 6: Unarchive not available in menu');
  504 |         }
  505 | 
  506 |         Logger.info('AUT_DOC_021 PASSED: Archive/unarchive behavior verified');
  507 |     });
  508 | });
  509 | 
  510 | // ============================================================
  511 | // === document-count-assign.spec.ts
  512 | // ============================================================
  513 | test.describe('Document - Count Update on Assign', () => {
  514 |     let loginPage: ProviderLoginPage;
  515 |     let docPage: DocumentLibraryPage;
  516 |     const { providerCredentials, providerPortalUrl } = getEnvironmentConfig();
  517 | 
  518 |     test.beforeEach(async ({ page }) => {
  519 |         loginPage = new ProviderLoginPage(page);
  520 |         docPage = new DocumentLibraryPage(page);
  521 |         await page.goto(providerPortalUrl);
  522 |         await loginPage.login(providerCredentials.username, providerCredentials.password);
  523 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  524 |     });
  525 | 
  526 |     test('AUT_DOC_019 - Verify document count increases after upload and assignment', async ({ page, createEnrolledPatient }) => {
  527 |         test.setTimeout(360000);
  528 |         Logger.step('Test: Document count update on assign');
  529 | 
  530 |         // Seed our own CCM patient (the shared "Automation" patient was deleted).
  531 |         const patient = await createEnrolledPatient({ state: 'Active', program: 'CCM' });
  532 | 
  533 |         // Step 1: Upload a unique document
  534 |         await docPage.navigateToDocumentLibrary();
  535 |         await docPage.clickFolder('Education');
  536 | 
  537 |         const ts = Date.now();
  538 |         const fn = `CountDoc ${ts}`;
  539 |         await docPage.uploadDocument({
  540 |             tag: 'Education', speciality: 'Cardiologist', fileName: fn,
  541 |             filePath: `${docsPath}/4mb.jpg`
  542 |         });
  543 |         Logger.info(`Step 1 ✓: Uploaded "${fn}"`);
  544 | 
  545 |         // Step 2: Verify document exists in folder
  546 |         await docPage.navigateToDocumentLibrary();
  547 |         await docPage.clickFolder('Education');
  548 |         await settle(page, 2000);
  549 |         await docPage.searchDocument(fn);
  550 |         expect(await docPage.isDocumentInList(fn), 'Document should be in Education folder').toBeTruthy();
  551 |         Logger.info('Step 2 ✓: Document found in Education folder');
  552 | 
  553 |         // Step 3: Assign to patient
  554 |         await docPage.assignDocumentToPatient(0, patient.lastName);
  555 |         Logger.info('Step 3 ✓: Document assigned to Automation, Test');
  556 | 
  557 |         // Step 4: Verify in patient charting — document count increased
  558 |         const patientChart = new PatientChartPage(page);
  559 |         await patientChart.openPatientChartFromGlobalSearch(patient.displayName);
  560 |         await settle(page, 2000);
  561 |         await page.locator("button:has-text('CCM')").first().or(page.getByText('CCM', { exact: true }).first()).click();
  562 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  563 |         await settle(page, 2000);
  564 |         await page.locator("button:has-text('Documents')").first().click();
  565 |         await settle(page, 2000);
  566 | 
  567 |         const educationFolder = page.locator("*:has-text('Education')").filter({ hasText: /^Education$/ });
  568 |         if (await educationFolder.count() > 0) {
  569 |             await educationFolder.first().click();
  570 |             await settle(page, 2000);
  571 |         }
  572 | 
  573 |         // Auto-retry until the assigned document renders in the Education folder.
  574 |         await expect(page.locator('main'),
  575 |             'Assigned document should appear in patient charting')
> 576 |             .toContainText(fn, { timeout: 15000 });
      |              ^ Error: Assigned document should appear in patient charting
  577 | 
  578 |         Logger.info(`AUT_DOC_019 PASSED: Document uploaded, assigned, and found in patient chart`);
  579 |     });
  580 | });
  581 | 
  582 | // ============================================================
  583 | // === document-count-delete.spec.ts
  584 | // ============================================================
  585 | test.describe('Document - Count Decrease on Delete', () => {
  586 |     let loginPage: ProviderLoginPage;
  587 |     let docPage: DocumentLibraryPage;
  588 |     const { providerCredentials, providerPortalUrl } = getEnvironmentConfig();
  589 | 
  590 |     test.beforeEach(async ({ page }) => {
  591 |         loginPage = new ProviderLoginPage(page);
  592 |         docPage = new DocumentLibraryPage(page);
  593 |         await page.goto(providerPortalUrl);
  594 |         await loginPage.login(providerCredentials.username, providerCredentials.password);
  595 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  596 |     });
  597 | 
  598 |     test('AUT_DOC_020 - Verify document removed from folder after deletion', async ({ page }) => {
  599 |         test.setTimeout(300000);
  600 |         Logger.step('Test: Document removed after delete');
  601 | 
  602 |         // Upload a document
  603 |         await docPage.navigateToDocumentLibrary();
  604 |         await docPage.clickFolder('Education');
  605 | 
  606 |         const ts = Date.now();
  607 |         const fn = `DelCount ${ts}`;
  608 |         await docPage.uploadDocument({
  609 |             tag: 'Education', speciality: 'Cardiologist', fileName: fn,
  610 |             filePath: `${docsPath}/4mb.jpg`
  611 |         });
  612 |         Logger.info(`Uploaded: ${fn}`);
  613 | 
  614 |         // Verify it exists
  615 |         await docPage.navigateToDocumentLibrary();
  616 |         await docPage.clickFolder('Education');
  617 |         await settle(page, 2000);
  618 |         await docPage.searchDocument(fn);
  619 |         expect(await docPage.isDocumentInList(fn), 'Document should exist before delete').toBeTruthy();
  620 |         Logger.info('✓ Document found before delete');
  621 | 
  622 |         // Delete it
  623 |         await docPage.deleteDocument(0);
  624 |         await docPage.confirmDelete();
  625 |         Logger.info('Document deleted');
  626 | 
  627 |         // Verify it's gone
  628 |         await docPage.navigateToDocumentLibrary();
  629 |         await docPage.clickFolder('Education');
  630 |         await settle(page, 2000);
  631 |         await docPage.searchDocument(fn);
  632 |         expect(await docPage.isDocumentInList(fn), 'Document should be removed after delete').toBeFalsy();
  633 |         Logger.info('✓ Document NOT found after delete');
  634 | 
  635 |         Logger.info('AUT_DOC_020 PASSED: Document removed from folder after deletion');
  636 |     });
  637 | });
  638 | 
  639 | // ============================================================
  640 | // === document-delete-workflow.spec.ts
  641 | // ============================================================
  642 | test.describe('Document - Delete Workflow', () => {
  643 |     let loginPage: ProviderLoginPage;
  644 |     let docPage: DocumentLibraryPage;
  645 |     const { providerCredentials, providerPortalUrl } = getEnvironmentConfig();
  646 | 
  647 |     test.beforeEach(async ({ page }) => {
  648 |         loginPage = new ProviderLoginPage(page);
  649 |         docPage = new DocumentLibraryPage(page);
  650 |         await page.goto(providerPortalUrl);
  651 |         await loginPage.login(providerCredentials.username, providerCredentials.password);
  652 |         await page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  653 |     });
  654 | 
  655 |     test('AUT_DOC_009 - Verify document delete with confirmation and removal from list', async ({ page }) => {
  656 |         test.setTimeout(300000);
  657 |         await docPage.navigateToDocumentLibrary();
  658 |         await docPage.clickFolder('Education');
  659 | 
  660 |         const ts = Date.now();
  661 |         const fn = `DelDoc ${ts}`;
  662 |         await docPage.uploadDocument({ tag: 'Education', speciality: 'Cardiologist', fileName: fn, filePath: `${docsPath}/4mb.jpg` });
  663 | 
  664 |         await docPage.navigateToDocumentLibrary();
  665 |         await docPage.clickFolder('Education');
  666 |         await settle(page, 2000);
  667 |         await docPage.searchDocument(fn);
  668 |         expect(await docPage.isDocumentInList(fn)).toBeTruthy();
  669 | 
  670 |         // isDocumentInList only checks page text; the actionable grid row (with
  671 |         // the MoreVert action icon) can lag a freshly-uploaded doc's search
  672 |         // result, so deleteDocument(0) could hit a not-yet-rendered row. Poll —
  673 |         // re-searching each round — until the action icon is present.
  674 |         let rowReady = false;
  675 |         for (let i = 0; i < 6 && !rowReady; i++) {
  676 |             rowReady = await page.locator("[data-testid='MoreVertIcon']").first()
```