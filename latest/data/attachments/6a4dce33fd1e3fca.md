# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/documents/documents-full-workflow.spec.ts >> Document Library - Upload >> AUT_DOC_001 - E2E Document Upload - Upload to Education folder with all fields, verify in correct folder
- Location: tests/web/provider-portal/documents/documents-full-workflow.spec.ts:1491:9

# Error details

```
Error: ENOENT: no such file or directory, stat '/__w/Unity-Health-Automation/Unity-Health-Automation/C:/Users/TTPL-LNVE16-0380/Desktop/Docs/4-mb-example-file (1).pdf'
```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e4]:
    - banner [ref=e5]:
      - generic [ref=e7]:
        - img [ref=e9]
        - generic [ref=e10]:
          - generic [ref=e13]:
            - img [ref=e15]
            - combobox [ref=e17]
            - button [ref=e19] [cursor=pointer]:
              - img [ref=e20]
            - group
          - button [ref=e22] [cursor=pointer]:
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
            - generic [ref=e58]: "309"
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
        - img [ref=e122]
      - listitem [ref=e125] [cursor=pointer]:
        - img [ref=e127]
    - main [ref=e129]:
      - generic [ref=e131]:
        - generic [ref=e132]:
          - heading [level=5] [ref=e133]: Documents
          - generic [ref=e134]:
            - generic [ref=e135] [cursor=pointer]:
              - generic [ref=e136]:
                - checkbox [ref=e137]
                - img [ref=e138]
              - generic [ref=e140]: Show Archived
            - generic [ref=e143]:
              - img [ref=e145]
              - textbox [ref=e147]:
                - /placeholder: Type here to search
              - group
            - button [ref=e148] [cursor=pointer]:
              - img [ref=e149]
              - text: Upload Material
        - navigation [ref=e151]:
          - list [ref=e152]:
            - listitem [ref=e153]:
              - heading [level=6] [ref=e154] [cursor=pointer]: Home
            - listitem [ref=e155]: ›
            - listitem [ref=e156]:
              - heading [level=6] [ref=e157] [cursor=pointer]: Education
        - generic [ref=e161]:
          - generic [ref=e162]:
            - generic [ref=e164]: "No"
            - generic [ref=e166]: Speciality
            - generic [ref=e168]: File Name
            - generic [ref=e170]: Tag
            - generic [ref=e172]: Type
            - generic [ref=e174]: Modified
            - generic [ref=e176]: Modified By
            - generic [ref=e178]: Actions
          - generic [ref=e179]:
            - generic [ref=e181] [cursor=pointer]: "01"
            - generic [ref=e183] [cursor=pointer]: Cardiologist
            - generic [ref=e185] [cursor=pointer]: UnarcAssign 1778657767676
            - generic [ref=e187] [cursor=pointer]: Education
            - generic [ref=e189] [cursor=pointer]: Image
            - generic [ref=e191] [cursor=pointer]: 05-13-2026
            - generic [ref=e193] [cursor=pointer]: chirag kumar
            - img [ref=e198] [cursor=pointer]
          - generic [ref=e200]:
            - generic [ref=e202] [cursor=pointer]: "02"
            - generic [ref=e204] [cursor=pointer]: Cardiologist
            - generic [ref=e206] [cursor=pointer]: TagEducation 1778657672060
            - generic [ref=e208] [cursor=pointer]: Education
            - generic [ref=e210] [cursor=pointer]: PDF
            - generic [ref=e212] [cursor=pointer]: 05-13-2026
            - generic [ref=e214] [cursor=pointer]: chirag kumar
            - img [ref=e219] [cursor=pointer]
          - generic [ref=e221]:
            - generic [ref=e223] [cursor=pointer]: "03"
            - generic [ref=e225] [cursor=pointer]: Cardiologist
            - generic [ref=e227] [cursor=pointer]: SigNotes 1778657612960
            - generic [ref=e229] [cursor=pointer]: Education
            - generic [ref=e231] [cursor=pointer]: Image
            - generic [ref=e233] [cursor=pointer]: 05-13-2026
            - generic [ref=e235] [cursor=pointer]: chirag kumar
            - img [ref=e240] [cursor=pointer]
          - generic [ref=e242]:
            - generic [ref=e244] [cursor=pointer]: "04"
            - generic [ref=e246] [cursor=pointer]: Cardiologist
            - generic [ref=e248] [cursor=pointer]: SearchMe 1778657583280
            - generic [ref=e250] [cursor=pointer]: Education
            - generic [ref=e252] [cursor=pointer]: Image
            - generic [ref=e254] [cursor=pointer]: 05-13-2026
            - generic [ref=e256] [cursor=pointer]: chirag kumar
            - img [ref=e261] [cursor=pointer]
          - generic [ref=e263]:
            - generic [ref=e265] [cursor=pointer]: "05"
            - generic [ref=e267] [cursor=pointer]: Cardiologist
            - generic [ref=e269] [cursor=pointer]: EduOnly 1778657537421
            - generic [ref=e271] [cursor=pointer]: Education
            - generic [ref=e273] [cursor=pointer]: Image
            - generic [ref=e275] [cursor=pointer]: 05-13-2026
            - generic [ref=e277] [cursor=pointer]: chirag kumar
            - img [ref=e282] [cursor=pointer]
          - generic [ref=e284]:
            - generic [ref=e286] [cursor=pointer]: "06"
            - generic [ref=e288] [cursor=pointer]: Cardiologist
            - generic [ref=e290] [cursor=pointer]: FEducation 1778657436399
            - generic [ref=e292] [cursor=pointer]: Education
            - generic [ref=e294] [cursor=pointer]: PDF
            - generic [ref=e296] [cursor=pointer]: 05-13-2026
            - generic [ref=e298] [cursor=pointer]: chirag kumar
            - img [ref=e303] [cursor=pointer]
          - generic [ref=e305]:
            - generic [ref=e307] [cursor=pointer]: "07"
            - generic [ref=e309] [cursor=pointer]: Cardiologist
            - generic [ref=e311] [cursor=pointer]: MultiAssign 1778657383020
            - generic [ref=e313] [cursor=pointer]: Education
            - generic [ref=e315] [cursor=pointer]: PDF
            - generic [ref=e317] [cursor=pointer]: 05-13-2026
            - generic [ref=e319] [cursor=pointer]: chirag kumar
            - img [ref=e324] [cursor=pointer]
          - generic [ref=e326]:
            - generic [ref=e328] [cursor=pointer]: "08"
            - generic [ref=e330] [cursor=pointer]: Pediatrician
            - generic [ref=e332] [cursor=pointer]: PNG_Upload 1778657303845
            - generic [ref=e334] [cursor=pointer]: Education
            - generic [ref=e336] [cursor=pointer]: Image
            - generic [ref=e338] [cursor=pointer]: 05-13-2026
            - generic [ref=e340] [cursor=pointer]: chirag kumar
            - img [ref=e345] [cursor=pointer]
          - generic [ref=e347]:
            - generic [ref=e349] [cursor=pointer]: "09"
            - generic [ref=e351] [cursor=pointer]: Cardiologist
            - generic [ref=e353] [cursor=pointer]: PDF_Upload 1778657303845
            - generic [ref=e355] [cursor=pointer]: Education
            - generic [ref=e357] [cursor=pointer]: PDF
            - generic [ref=e359] [cursor=pointer]: 05-13-2026
            - generic [ref=e361] [cursor=pointer]: chirag kumar
            - img [ref=e366] [cursor=pointer]
          - generic [ref=e368]:
            - generic [ref=e370] [cursor=pointer]: "10"
            - generic [ref=e372] [cursor=pointer]: Cardiologist
            - generic [ref=e374] [cursor=pointer]: CountDoc 1778657190688
            - generic [ref=e376] [cursor=pointer]: Education
            - generic [ref=e378] [cursor=pointer]: Image
            - generic [ref=e380] [cursor=pointer]: 05-13-2026
            - generic [ref=e382] [cursor=pointer]: chirag kumar
            - img [ref=e387] [cursor=pointer]
          - generic [ref=e389]:
            - generic [ref=e391] [cursor=pointer]: "11"
            - generic [ref=e393] [cursor=pointer]: Cardiologist
            - generic [ref=e395] [cursor=pointer]: ArcRestore 1778657134076
            - generic [ref=e397] [cursor=pointer]: Education
            - generic [ref=e399] [cursor=pointer]: Image
            - generic [ref=e401] [cursor=pointer]: 05-13-2026
            - generic [ref=e403] [cursor=pointer]: chirag kumar
            - img [ref=e408] [cursor=pointer]
          - generic [ref=e410]:
            - generic [ref=e412] [cursor=pointer]: "12"
            - generic [ref=e414] [cursor=pointer]: Cardiologist
            - generic [ref=e416] [cursor=pointer]: Consistency 1778657068205
            - generic [ref=e418] [cursor=pointer]: Education
            - generic [ref=e420] [cursor=pointer]: Image
            - generic [ref=e422] [cursor=pointer]: 05-13-2026
            - generic [ref=e424] [cursor=pointer]: chirag kumar
            - img [ref=e429] [cursor=pointer]
          - generic [ref=e431]:
            - generic [ref=e433] [cursor=pointer]: "13"
            - generic [ref=e435] [cursor=pointer]: Cardiologist
            - generic [ref=e437] [cursor=pointer]: AssignDoc 1778657020346
            - generic [ref=e439] [cursor=pointer]: Education
            - generic [ref=e441] [cursor=pointer]: PDF
            - generic [ref=e443] [cursor=pointer]: 05-13-2026
            - generic [ref=e445] [cursor=pointer]: chirag kumar
            - img [ref=e450] [cursor=pointer]
          - generic [ref=e452]:
            - generic [ref=e454] [cursor=pointer]: "14"
            - generic [ref=e456] [cursor=pointer]: Cardiologist
            - generic [ref=e458] [cursor=pointer]: Education 1778510641283
            - generic [ref=e460] [cursor=pointer]: Education
            - generic [ref=e462] [cursor=pointer]: PDF
            - generic [ref=e464] [cursor=pointer]: 05-11-2026
            - generic [ref=e466] [cursor=pointer]: chirag kumar
            - img [ref=e471] [cursor=pointer]
          - generic [ref=e473]:
            - generic [ref=e475] [cursor=pointer]: "15"
            - generic [ref=e477] [cursor=pointer]: Cardiologist
            - generic [ref=e479] [cursor=pointer]: AutoDoc 1778510605185
            - generic [ref=e481] [cursor=pointer]: Education
            - generic [ref=e483] [cursor=pointer]: PDF
            - generic [ref=e485] [cursor=pointer]: 05-11-2026
            - generic [ref=e487] [cursor=pointer]: chirag kumar
            - img [ref=e492] [cursor=pointer]
          - generic [ref=e494]:
            - generic [ref=e496] [cursor=pointer]: "16"
            - generic [ref=e498] [cursor=pointer]: Cardiologist
            - generic [ref=e500] [cursor=pointer]: UnarcAssign 1778510508574
            - generic [ref=e502] [cursor=pointer]: Education
            - generic [ref=e504] [cursor=pointer]: Image
            - generic [ref=e506] [cursor=pointer]: 05-11-2026
            - generic [ref=e508] [cursor=pointer]: chirag kumar
            - img [ref=e513] [cursor=pointer]
          - generic [ref=e515]:
            - generic [ref=e517] [cursor=pointer]: "17"
            - generic [ref=e519] [cursor=pointer]: Cardiologist
            - generic [ref=e521] [cursor=pointer]: TagEducation 1778510394510
            - generic [ref=e523] [cursor=pointer]: Education
            - generic [ref=e525] [cursor=pointer]: PDF
            - generic [ref=e527] [cursor=pointer]: 05-11-2026
            - generic [ref=e529] [cursor=pointer]: chirag kumar
            - img [ref=e534] [cursor=pointer]
          - generic [ref=e536]:
            - generic [ref=e538] [cursor=pointer]: "18"
            - generic [ref=e540] [cursor=pointer]: Cardiologist
            - generic [ref=e542] [cursor=pointer]: SigNotes 1778510312935
            - generic [ref=e544] [cursor=pointer]: Education
            - generic [ref=e546] [cursor=pointer]: Image
            - generic [ref=e548] [cursor=pointer]: 05-11-2026
            - generic [ref=e550] [cursor=pointer]: chirag kumar
            - img [ref=e555] [cursor=pointer]
          - generic [ref=e557]:
            - generic [ref=e559] [cursor=pointer]: "19"
            - generic [ref=e561] [cursor=pointer]: Cardiologist
            - generic [ref=e563] [cursor=pointer]: SearchMe 1778510265330
            - generic [ref=e565] [cursor=pointer]: Education
            - generic [ref=e567] [cursor=pointer]: Image
            - generic [ref=e569] [cursor=pointer]: 05-11-2026
            - generic [ref=e571] [cursor=pointer]: chirag kumar
            - img [ref=e576] [cursor=pointer]
          - generic [ref=e578]:
            - generic [ref=e580] [cursor=pointer]: "20"
            - generic [ref=e582] [cursor=pointer]: Cardiologist
            - generic [ref=e584] [cursor=pointer]: EduOnly 1778510208237
            - generic [ref=e586] [cursor=pointer]: Education
            - generic [ref=e588] [cursor=pointer]: Image
            - generic [ref=e590] [cursor=pointer]: 05-11-2026
            - generic [ref=e592] [cursor=pointer]: chirag kumar
            - img [ref=e597] [cursor=pointer]
          - generic [ref=e599]:
            - generic [ref=e601] [cursor=pointer]: "21"
            - generic [ref=e603] [cursor=pointer]: Cardiologist
            - generic [ref=e605] [cursor=pointer]: FEducation 1778510081111
            - generic [ref=e607] [cursor=pointer]: Education
            - generic [ref=e609] [cursor=pointer]: PDF
            - generic [ref=e611] [cursor=pointer]: 05-11-2026
            - generic [ref=e613] [cursor=pointer]: chirag kumar
            - img [ref=e618] [cursor=pointer]
          - generic [ref=e620]:
            - generic [ref=e622] [cursor=pointer]: "22"
            - generic [ref=e624] [cursor=pointer]: Cardiologist
            - generic [ref=e626] [cursor=pointer]: MultiAssign 1778510011999
            - generic [ref=e628] [cursor=pointer]: Education
            - generic [ref=e630] [cursor=pointer]: PDF
            - generic [ref=e632] [cursor=pointer]: 05-11-2026
            - generic [ref=e634] [cursor=pointer]: chirag kumar
            - img [ref=e639] [cursor=pointer]
          - generic [ref=e641]:
            - generic [ref=e643] [cursor=pointer]: "23"
            - generic [ref=e645] [cursor=pointer]: Pediatrician
            - generic [ref=e647] [cursor=pointer]: PNG_Upload 1778509911680
            - generic [ref=e649] [cursor=pointer]: Education
            - generic [ref=e651] [cursor=pointer]: Image
            - generic [ref=e653] [cursor=pointer]: 05-11-2026
            - generic [ref=e655] [cursor=pointer]: chirag kumar
            - img [ref=e660] [cursor=pointer]
          - generic [ref=e662]:
            - generic [ref=e664] [cursor=pointer]: "24"
            - generic [ref=e666] [cursor=pointer]: Cardiologist
            - generic [ref=e668] [cursor=pointer]: PDF_Upload 1778509911680
            - generic [ref=e670] [cursor=pointer]: Education
            - generic [ref=e672] [cursor=pointer]: PDF
            - generic [ref=e674] [cursor=pointer]: 05-11-2026
            - generic [ref=e676] [cursor=pointer]: chirag kumar
            - img [ref=e681] [cursor=pointer]
          - generic [ref=e683]:
            - generic [ref=e685] [cursor=pointer]: "25"
            - generic [ref=e687] [cursor=pointer]: Cardiologist
            - generic [ref=e689] [cursor=pointer]: CountDoc 1778509758014
            - generic [ref=e691] [cursor=pointer]: Education
            - generic [ref=e693] [cursor=pointer]: Image
            - generic [ref=e695] [cursor=pointer]: 05-11-2026
            - generic [ref=e697] [cursor=pointer]: chirag kumar
            - img [ref=e702] [cursor=pointer]
          - generic [ref=e704]:
            - progressbar [ref=e705]:
              - img [ref=e706]
            - generic [ref=e708]: Loading more...
  - generic [ref=e712]:
    - generic [ref=e713]:
      - heading "UPLOAD FILE" [level=5] [ref=e716]
      - generic [ref=e717]:
        - button "Cancel" [ref=e718] [cursor=pointer]:
          - heading "Cancel" [level=6] [ref=e719]
        - button "Upload" [disabled]:
          - heading "Upload" [level=6]
    - generic [ref=e721]:
      - generic [ref=e722]:
        - generic [ref=e724]: Tag*
        - generic [ref=e725]:
          - combobox "Education" [ref=e726] [cursor=pointer]
          - textbox: EDUCATION
          - img
          - group
      - generic [ref=e727]:
        - generic [ref=e729]: Speciality*
        - generic [ref=e730]:
          - combobox "Cardiologist" [ref=e731] [cursor=pointer]
          - textbox: "[object Object]"
          - img
          - group
      - generic [ref=e732]:
        - generic [ref=e734]: File Name*
        - textbox "Enter Note" [active] [ref=e736]: AutoDoc 1778657864857
      - generic [ref=e737]:
        - paragraph [ref=e738]: Upload Result*
        - paragraph [ref=e739]: "Upload Your File,(eg: PNG,JPEG,PDF,MP4)"
        - generic [ref=e742] [cursor=pointer]:
          - heading "Drop Here Image" [level=6] [ref=e745]:
            - img [ref=e746]
            - text: Drop Here Image
          - heading "No File Selected" [level=6] [ref=e749]
      - textbox "Enter Note" [ref=e752]
      - generic [ref=e754] [cursor=pointer]:
        - generic [ref=e755]:
          - checkbox "Signature Required" [ref=e756]
          - img [ref=e757]
        - generic [ref=e759]: Signature Required
```

# Test source

```ts
  54  | 
  55  |         // Otherwise click sidebar
  56  |         await this.page.locator(this.documentLibrarySidebarLink).first().waitFor({ state: 'visible', timeout: 10000 });
  57  |         await this.page.locator(this.documentLibrarySidebarLink).first().click();
  58  |         await this.page.waitForLoadState('networkidle');
  59  |         await this.page.waitForTimeout(1500);
  60  |         Logger.info('Navigated to Document Library via sidebar');
  61  |     }
  62  | 
  63  |     async verifyOnDocumentLibrary(): Promise<boolean> {
  64  |         try {
  65  |             await this.page.locator(this.documentsPageTitle).first().waitFor({ state: 'visible', timeout: 10000 });
  66  |             return true;
  67  |         } catch {
  68  |             return false;
  69  |         }
  70  |     }
  71  | 
  72  |     // =============================================
  73  |     // FOLDERS
  74  |     // =============================================
  75  | 
  76  |     async clickFolder(folderName: string): Promise<void> {
  77  |         Logger.step(`Clicking folder: ${folderName}`);
  78  |         const folderLocators: Record<string, string> = {
  79  |             'Home Exercise': this.homeExerciseFolder,
  80  |             'Education': this.educationFolder,
  81  |             'Challenges': this.challengesFolder,
  82  |             'Care Plan': this.carePlanFolder,
  83  |             'Consent': this.consentFolder
  84  |         };
  85  |         const selector = folderLocators[folderName];
  86  |         if (selector) {
  87  |             await this.page.locator(selector).first().click();
  88  |             await this.page.waitForLoadState('networkidle');
  89  |             await this.page.waitForTimeout(1500);
  90  |             Logger.info(`Opened folder: ${folderName}`);
  91  |         }
  92  |     }
  93  | 
  94  |     async getFolderNames(): Promise<string[]> {
  95  |         const folders = ['Home Exercise', 'Education', 'Challenges', 'Care Plan', 'Consent'];
  96  |         const visible: string[] = [];
  97  |         for (const f of folders) {
  98  |             const loc = this.page.locator(`//*[text()='${f}']`);
  99  |             if (await loc.isVisible().catch(() => false)) visible.push(f);
  100 |         }
  101 |         Logger.info(`Visible folders: ${visible.join(', ')}`);
  102 |         return visible;
  103 |     }
  104 | 
  105 |     // =============================================
  106 |     // UPLOAD MATERIAL
  107 |     // =============================================
  108 | 
  109 |     async clickUploadMaterial(): Promise<void> {
  110 |         Logger.step('Clicking Upload Material button');
  111 |         await this.page.locator(this.uploadMaterialButton).click();
  112 |         await this.page.waitForTimeout(1500);
  113 |         Logger.info('Upload Material form opened');
  114 |     }
  115 | 
  116 |     async isUploadFormVisible(): Promise<boolean> {
  117 |         try {
  118 |             await this.page.locator(this.uploadFormTitle).waitFor({ state: 'visible', timeout: 5000 });
  119 |             return true;
  120 |         } catch {
  121 |             return false;
  122 |         }
  123 |     }
  124 | 
  125 |     async selectTag(tagName: string): Promise<void> {
  126 |         Logger.step(`Selecting tag: ${tagName}`);
  127 |         const comboboxes = this.page.locator(this.tagDropdown);
  128 |         await comboboxes.first().click();
  129 |         await this.page.waitForTimeout(800);
  130 |         await this.page.getByRole('option', { name: tagName }).click();
  131 |         await this.page.waitForTimeout(500);
  132 |         Logger.info(`Tag selected: ${tagName}`);
  133 |     }
  134 | 
  135 |     async selectSpeciality(speciality: string): Promise<void> {
  136 |         Logger.step(`Selecting speciality: ${speciality}`);
  137 |         const comboboxes = this.page.locator(this.tagDropdown);
  138 |         await comboboxes.nth(1).click();
  139 |         await this.page.waitForTimeout(800);
  140 |         await this.page.getByRole('option', { name: speciality, exact: true }).click();
  141 |         await this.page.waitForTimeout(500);
  142 |         Logger.info(`Speciality selected: ${speciality}`);
  143 |     }
  144 | 
  145 |     async fillFileName(name: string): Promise<void> {
  146 |         Logger.step(`Filling file name: ${name}`);
  147 |         await this.page.locator(this.fileNameInput).first().fill(name);
  148 |         await this.page.waitForTimeout(300);
  149 |     }
  150 | 
  151 |     async uploadFile(filePath: string): Promise<void> {
  152 |         Logger.step(`Uploading file: ${filePath}`);
  153 |         const absolutePath = path.resolve(filePath);
> 154 |         await this.page.locator(this.fileInput).setInputFiles(absolutePath);
      |         ^ Error: ENOENT: no such file or directory, stat '/__w/Unity-Health-Automation/Unity-Health-Automation/C:/Users/TTPL-LNVE16-0380/Desktop/Docs/4-mb-example-file (1).pdf'
  155 | 
  156 |         // Wait for file upload to complete
  157 |         Logger.info('Waiting for file upload to complete...');
  158 | 
  159 |         // Wait until progress bar disappears (up to 2 minutes for large files)
  160 |         await this.page.locator("[role='progressbar']")
  161 |             .waitFor({ state: 'hidden', timeout: 120000 }).catch(() => {});
  162 | 
  163 |         // Wait until Upload button becomes enabled
  164 |         await this.page.locator("//button[.//h6[text()='Upload']]")
  165 |             .waitFor({ state: 'visible', timeout: 30000 }).catch(() => {});
  166 | 
  167 |         // Extra wait for UI to stabilize
  168 |         await this.page.waitForTimeout(1000);
  169 |         Logger.info(`File upload completed: ${absolutePath}`);
  170 |     }
  171 | 
  172 |     async fillDescription(description: string): Promise<void> {
  173 |         Logger.step(`Filling description: ${description}`);
  174 |         await this.page.locator(this.descriptionTextarea).first().fill(description);
  175 |         await this.page.waitForTimeout(300);
  176 |     }
  177 | 
  178 |     async clickUpload(): Promise<void> {
  179 |         Logger.step('Clicking Upload button');
  180 | 
  181 |         // Wait for the Upload button to become enabled (not disabled)
  182 |         const uploadBtn = this.page.locator(this.uploadButton).last();
  183 |         await uploadBtn.waitFor({ state: 'visible', timeout: 30000 });
  184 | 
  185 |         // Wait until button is no longer disabled
  186 |         await this.page.waitForFunction(() => {
  187 |             const btn = document.querySelector('button[disabled]');
  188 |             const uploadBtns = Array.from(document.querySelectorAll('button'));
  189 |             const uploadBtn = uploadBtns.find(b => b.textContent?.trim() === 'Upload' && !b.textContent?.includes('Material'));
  190 |             return uploadBtn && !uploadBtn.disabled;
  191 |         }, { timeout: 120000 });
  192 | 
  193 |         Logger.info('Upload button enabled — clicking');
  194 |         await uploadBtn.click();
  195 |         await this.page.waitForTimeout(2000);
  196 | 
  197 |         // Wait for toast
  198 |         const toast = this.page.locator(this.toastMessage);
  199 |         await toast.first().waitFor({ state: 'visible', timeout: 10000 }).catch(() => {});
  200 | 
  201 |         // Wait for form to close
  202 |         await this.page.locator(this.uploadFormTitle).waitFor({ state: 'hidden', timeout: 10000 }).catch(async () => {
  203 |             Logger.info('Upload form still open — pressing Escape');
  204 |             await this.page.keyboard.press('Escape');
  205 |             await this.page.waitForTimeout(1000);
  206 |         });
  207 | 
  208 |         await this.page.waitForTimeout(1000);
  209 |         Logger.info('Upload completed');
  210 |     }
  211 | 
  212 |     async clickCancel(): Promise<void> {
  213 |         Logger.step('Clicking Cancel');
  214 |         await this.page.locator(this.cancelButton).first().click();
  215 |         await this.page.waitForTimeout(500);
  216 |     }
  217 | 
  218 |     async checkSignatureRequired(): Promise<void> {
  219 |         Logger.step('Checking Signature Required checkbox');
  220 |         const checkbox = this.page.locator(this.signatureCheckbox).first();
  221 |         await checkbox.click();
  222 |         await this.page.waitForTimeout(500);
  223 |         Logger.info('Signature Required checked');
  224 |     }
  225 | 
  226 |     async fillNotes(notes: string): Promise<void> {
  227 |         Logger.step(`Filling notes: ${notes}`);
  228 |         const notesField = this.page.locator("//textarea[@placeholder='Enter Note']").last();
  229 |         await notesField.fill(notes);
  230 |         await this.page.waitForTimeout(300);
  231 |         Logger.info('Notes filled');
  232 |     }
  233 | 
  234 |     /**
  235 |      * Upload a document with all fields.
  236 |      */
  237 |     async uploadDocument(data: {
  238 |         tag: string;
  239 |         speciality: string;
  240 |         fileName: string;
  241 |         filePath: string;
  242 |         description?: string;
  243 |         signatureRequired?: boolean;
  244 |         notes?: string;
  245 |     }): Promise<void> {
  246 |         Logger.step(`Uploading document: ${data.fileName}`);
  247 | 
  248 |         await this.clickUploadMaterial();
  249 |         await this.selectTag(data.tag);
  250 |         await this.selectSpeciality(data.speciality);
  251 |         await this.fillFileName(data.fileName);
  252 |         await this.uploadFile(data.filePath);
  253 | 
  254 |         if (data.description) {
```