# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/library/care-plan.spec.ts >> Care Plan Flow >> should not save care plan when cancelled during creation
- Location: tests/web/provider-portal/library/care-plan.spec.ts:652:9

# Error details

```
TimeoutError: locator.waitFor: Timeout 10000ms exceeded.
Call log:
  - waiting for locator('//h2[text()=\'Cancel Confirmation\']/ancestor::div[contains(@class,\'MuiPaper\')]//p') to be visible

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
                - generic [ref=f1e96]: "170"
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
              - checkbox "Show Archived" [checked] [ref=f1e241]
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
            - generic "Archive Plan 1787294145928" [ref=f1e278] [cursor=pointer]
            - generic "A001" [ref=f1e281]: A001-Chole...
            - generic "08-21-2026, 06:36 AM" [ref=f1e283] [cursor=pointer]
            - generic "PROVIDER" [ref=f1e285] [cursor=pointer]
            - generic "ACTIVE" [ref=f1e287] [cursor=pointer]
            - generic [ref=f1e291] [cursor=pointer]
          - generic [ref=f1e294]:
            - generic "02" [ref=f1e296] [cursor=pointer]
            - generic "Archive Plan 1787561213178" [ref=f1e298] [cursor=pointer]
            - generic "A001" [ref=f1e301]: A001-Chole...
            - generic "08-24-2026, 08:47 AM" [ref=f1e303] [cursor=pointer]
            - generic "PROVIDER" [ref=f1e305] [cursor=pointer]
            - generic "ACTIVE" [ref=f1e307] [cursor=pointer]
            - generic [ref=f1e311] [cursor=pointer]
          - generic [ref=f1e314]:
            - progressbar [ref=f1e315]
            - generic [ref=f1e318]: Loading...
    - button [ref=f1e320] [cursor=pointer]
    - button [ref=f1e324] [cursor=pointer]
  - alert [ref=f1e327]:
    - generic [ref=f1e331]: CarePlan deleted successfully!
    - button "Close" [ref=f1e333] [cursor=pointer]
```

# Test source

```ts
  642 |         Logger.info(`Minimal care plan '${carePlanName}' created`);
  643 |     }
  644 | 
  645 |     /**
  646 |      * Edits an existing care plan: updates the name and navigates through wizard to save.
  647 |      * Edit opens Step 1 (section checklist), then steps through Overview and other sections.
  648 |      */
  649 |     async editCarePlan(oldName: string, newName: string): Promise<void> {
  650 |         Logger.step(`Editing care plan from '${oldName}' to '${newName}'`);
  651 | 
  652 |         await this.clickEditFromMenu(oldName);
  653 | 
  654 |         // Step 1: Update the name
  655 |         await this.carePlanNameInput.waitFor({ state: 'visible', timeout: 10000 });
  656 |         await this.carePlanNameInput.fill('');
  657 |         await this.carePlanNameInput.fill(newName);
  658 | 
  659 |         // Navigate through all wizard steps clicking Next until Finish appears.
  660 |         // If neither Next nor Finish is visible momentarily (validation in flight
  661 |         // or DOM transition), wait briefly and re-check before giving up — the
  662 |         // previous version broke out and then immediately tried clickFinish,
  663 |         // which would throw if Finish hadn't rendered yet.
  664 |         let maxSteps = 15;
  665 |         while (maxSteps > 0) {
  666 |             if (await this.isFinishButtonVisible()) break;
  667 |             if (await this.isNextButtonVisible()) {
  668 |                 await this.clickNext();
  669 |             } else {
  670 |                 // Stall — let the page settle, then re-probe.
  671 |                 await this.page.waitForTimeout(1200);
  672 |                 if (await this.isFinishButtonVisible()) break;
  673 |                 if (await this.isNextButtonVisible()) {
  674 |                     await this.clickNext();
  675 |                     maxSteps--;
  676 |                     continue;
  677 |                 }
  678 |                 break;
  679 |             }
  680 |             maxSteps--;
  681 |         }
  682 | 
  683 |         // Final wait for Finish — it can fade in during the last wizard transition.
  684 |         await this.page.locator(this.finishBtn).first()
  685 |             .waitFor({ state: 'visible', timeout: 10000 })
  686 |             .catch(() => {});
  687 |         await this.clickFinish();
  688 |         Logger.info(`Care plan updated from '${oldName}' to '${newName}'`);
  689 |     }
  690 | 
  691 |     // =============================================
  692 |     // ARCHIVE
  693 |     // =============================================
  694 | 
  695 |     async clickArchiveFromMenu(carePlanName: string): Promise<void> {
  696 |         Logger.step(`Clicking Archive for: ${carePlanName}`);
  697 |         await this.searchCarePlan(carePlanName);
  698 |         await this.openActionMenu(carePlanName);
  699 |         await this.page.locator(this.archiveBtn).click({ timeout: 10000 });
  700 |         await this.page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  701 |         await this.page.waitForTimeout(2000);
  702 |         // Clear search to refresh the list after archive
  703 |         await this.clearSearch();
  704 |         Logger.info(`Care plan '${carePlanName}' archived`);
  705 |     }
  706 | 
  707 |     async toggleShowArchived(): Promise<void> {
  708 |         Logger.step('Toggling Show Archived checkbox');
  709 |         await this.showArchivedLabel.click();
  710 |         await this.page.waitForLoadState('networkidle', { timeout: 10000 }).catch(() => {});
  711 |         await this.page.waitForTimeout(2000);
  712 |         Logger.info('Show Archived toggled');
  713 |     }
  714 | 
  715 |     // =============================================
  716 |     // VIEW ONLY (PREVIEW CARE PLAN)
  717 |     // =============================================
  718 | 
  719 |     async clickViewOnlyFromMenu(carePlanName: string): Promise<void> {
  720 |         Logger.step(`Clicking View Only for: ${carePlanName}`);
  721 |         await this.searchCarePlan(carePlanName);
  722 |         await this.openActionMenu(carePlanName);
  723 |         await this.page.locator(this.viewOnlyBtn).click({ timeout: 10000 });
  724 |         await this.page.waitForTimeout(3000);
  725 |         Logger.info('Preview Care Plan page opened');
  726 |     }
  727 | 
  728 |     async isOnPreviewPage(): Promise<boolean> {
  729 |         return await this.page.locator('//*[self::h4 or self::h5 or self::h6][contains(translate(normalize-space(),"abcdefghijklmnopqrstuvwxyz","ABCDEFGHIJKLMNOPQRSTUVWXYZ"),"PREVIEW CARE PLAN")]').first().isVisible().catch(() => false);
  730 |     }
  731 | 
  732 |     async verifyPreviewContainsText(text: string): Promise<void> {
  733 |         await expect(this.page.getByText(text).first()).toBeVisible({ timeout: 10000 });
  734 |     }
  735 | 
  736 |     // =============================================
  737 |     // CANCEL CONFIRMATION DIALOG
  738 |     // =============================================
  739 | 
  740 |     async getCancelConfirmationMessage(): Promise<string> {
  741 |         const msg = this.page.locator("//h2[text()='Cancel Confirmation']/ancestor::div[contains(@class,'MuiPaper')]//p");
> 742 |         await msg.waitFor({ state: 'visible', timeout: 10000 });
      |                   ^ TimeoutError: locator.waitFor: Timeout 10000ms exceeded.
  743 |         return (await msg.textContent()) || '';
  744 |     }
  745 | 
  746 |     async confirmCancelDialog(): Promise<void> {
  747 |         Logger.step('Confirming cancel dialog (clicking Yes)');
  748 |         await this.page.locator(this.cancelConfirmationTitle).waitFor({ state: 'visible', timeout: 10000 });
  749 |         await this.page.locator(this.cancelConfirmYesBtn).click();
  750 |         await this.page.waitForTimeout(2000);
  751 |         Logger.info('Cancel confirmed');
  752 |     }
  753 | 
  754 |     async dismissCancelDialog(): Promise<void> {
  755 |         Logger.step('Dismissing cancel dialog (clicking No)');
  756 |         await this.page.locator(this.cancelConfirmationTitle).waitFor({ state: 'visible', timeout: 10000 });
  757 |         await this.page.locator(this.cancelConfirmNoBtn).click();
  758 |         await this.page.waitForTimeout(1000);
  759 |         Logger.info('Cancel dismissed');
  760 |     }
  761 | 
  762 |     async isCancelConfirmationVisible(): Promise<boolean> {
  763 |         return await this.page.locator(this.cancelConfirmationTitle).isVisible().catch(() => false);
  764 |     }
  765 | 
  766 |     // =============================================
  767 |     // TOAST MESSAGES
  768 |     // =============================================
  769 | 
  770 |     async getToastMessage(): Promise<string> {
  771 |         await this.toastMessage.first().waitFor({ state: 'visible', timeout: 10000 });
  772 |         return (await this.toastMessage.first().textContent()) || '';
  773 |     }
  774 | 
  775 |     async waitForToastWithText(expectedText: string): Promise<void> {
  776 |         Logger.step(`Waiting for toast message containing: ${expectedText}`);
  777 |         await this.page.locator(`.MuiSnackbar-root:has-text("${expectedText}")`).first().waitFor({ state: 'visible', timeout: 10000 });
  778 |         Logger.info(`Toast message found: ${expectedText}`);
  779 |     }
  780 | 
  781 |     // =============================================
  782 |     // LIST PAGE STATE CHECKS
  783 |     // =============================================
  784 | 
  785 |     async isOnListPage(): Promise<boolean> {
  786 |         return await this.createCarePlanBtn.isVisible().catch(() => false);
  787 |     }
  788 | 
  789 |     async getCarePlanStatus(carePlanName: string): Promise<string> {
  790 |         const row = this.page.locator(`//div[@aria-label='${carePlanName}']/ancestor::div[contains(@class,'css-187srpe')]`);
  791 |         const statusCell = row.locator('//*[text()="ACTIVE" or text()="DRAFT" or text()="ARCHIVED"]').first();
  792 |         return (await statusCell.textContent().catch(() => 'UNKNOWN')) || 'UNKNOWN';
  793 |     }
  794 | 
  795 |     // NOTE: care plans are NOT assigned from the library row's action menu
  796 |     // (which only offers View Only / Edit / Delete / Archive). They're
  797 |     // assigned from inside the patient chart's CCM → Care Plan tab via
  798 |     // the "Manage Plan" button. See `assignCarePlanToPatient` in
  799 |     // utils/care-plan-test-helpers.ts for the proven implementation.
  800 | }
  801 | 
```