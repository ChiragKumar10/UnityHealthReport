# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/patient-wallet/patient-documents-workflow.spec.ts >> Patient Wallet - Documents Full Workflow >> AUT_PT_DOC_001 - Complete document workflow in patient chart (13 scenarios)
- Location: tests/web/provider-portal/patient-wallet/patient-documents-workflow.spec.ts:25:9

# Error details

```
Error: ENOENT: no such file or directory, stat 'C:/Users/TTPL-LNVE16-0380/Desktop/Docs/4mb.jpg'
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
            - generic [ref=e58]: "305"
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
        - group [ref=e132]:
          - button [ref=e133] [cursor=pointer]: RPM
          - button [ref=e134] [cursor=pointer]: RTM
          - button [pressed] [ref=e135] [cursor=pointer]: CCM
          - button [ref=e136] [cursor=pointer]: PCM
        - generic [ref=e137]:
          - generic [ref=e139]:
            - img [ref=e141]
            - generic [ref=e144]:
              - generic [ref=e145]:
                - heading [level=5] [ref=e146]: Automation, Test
                - heading [level=6] [ref=e147]:
                  - text: Male | 12-12-2000 |
                  - heading [level=6] [ref=e148]: CCM - Enrolled 02-18-2026
              - generic [ref=e149]:
                - heading [level=6] [ref=e150]: User hasn't logged in
                - generic [ref=e151]:
                  - button [ref=e152] [cursor=pointer]:
                    - img [ref=e154]
                    - text: Profile
                  - img
          - generic [ref=e159]:
            - generic [ref=e160]:
              - paragraph [ref=e161]: Global Comment
              - button [ref=e162] [cursor=pointer]:
                - img [ref=e164]
                - text: New
            - generic [ref=e166]:
              - generic [ref=e167]:
                - paragraph [ref=e168]:
                  - img [ref=e169]
                  - text: PW-Mon comment 1776766181152
                - generic [ref=e171]:
                  - button [ref=e172] [cursor=pointer]:
                    - img [ref=e173]
                  - button [ref=e175] [cursor=pointer]:
                    - img [ref=e176]
              - generic [ref=e178]:
                - paragraph [ref=e179]:
                  - img [ref=e180]
                  - text: PW-Mon comment 1776765850233
                - generic [ref=e182]:
                  - button [ref=e183] [cursor=pointer]:
                    - img [ref=e184]
                  - button [ref=e186] [cursor=pointer]:
                    - img [ref=e187]
              - generic [ref=e189]:
                - paragraph [ref=e190]:
                  - img [ref=e191]
                  - text: PW-Mon comment 1776765558756
                - generic [ref=e193]:
                  - button [ref=e194] [cursor=pointer]:
                    - img [ref=e195]
                  - button [ref=e197] [cursor=pointer]:
                    - img [ref=e198]
              - generic [ref=e200]:
                - paragraph [ref=e201]:
                  - img [ref=e202]
                  - text: PW-Mon comment 1776765209049 edited
                - generic [ref=e204]:
                  - button [ref=e205] [cursor=pointer]:
                    - img [ref=e206]
                  - button [ref=e208] [cursor=pointer]:
                    - img [ref=e209]
              - generic [ref=e211]:
                - paragraph [ref=e212]:
                  - img [ref=e213]
                  - text: PW-Mon comment 1776764512792
                - generic [ref=e215]:
                  - button [ref=e216] [cursor=pointer]:
                    - img [ref=e217]
                  - button [ref=e219] [cursor=pointer]:
                    - img [ref=e220]
              - generic [ref=e222]:
                - paragraph [ref=e223]:
                  - img [ref=e224]
                  - text: PW-Mon comment 1776759686293 edited
                - generic [ref=e226]:
                  - button [ref=e227] [cursor=pointer]:
                    - img [ref=e228]
                  - button [ref=e230] [cursor=pointer]:
                    - img [ref=e231]
              - generic [ref=e233]:
                - paragraph [ref=e234]:
                  - img [ref=e235]
                  - text: PW-Mon comment 1776759364706 edited
                - generic [ref=e237]:
                  - button [ref=e238] [cursor=pointer]:
                    - img [ref=e239]
                  - button [ref=e241] [cursor=pointer]:
                    - img [ref=e242]
              - generic [ref=e244]:
                - paragraph [ref=e245]:
                  - img [ref=e246]
                  - text: PW-Mon comment 1776757434980
                - generic [ref=e248]:
                  - button [ref=e249] [cursor=pointer]:
                    - img [ref=e250]
                  - button [ref=e252] [cursor=pointer]:
                    - img [ref=e253]
              - generic [ref=e255]:
                - paragraph [ref=e256]:
                  - img [ref=e257]
                  - text: PW-Mon comment 1776756774368
                - generic [ref=e259]:
                  - button [ref=e260] [cursor=pointer]:
                    - img [ref=e261]
                  - button [ref=e263] [cursor=pointer]:
                    - img [ref=e264]
              - generic [ref=e266]:
                - paragraph [ref=e267]:
                  - img [ref=e268]
                  - text: PW-Mon comment 1776755946482
                - generic [ref=e270]:
                  - button [ref=e271] [cursor=pointer]:
                    - img [ref=e272]
                  - button [ref=e274] [cursor=pointer]:
                    - img [ref=e275]
              - generic [ref=e277]:
                - paragraph [ref=e278]:
                  - img [ref=e279]
                  - text: PW-Mon comment 1776755946482 edited
                - generic [ref=e281]:
                  - button [ref=e282] [cursor=pointer]:
                    - img [ref=e283]
                  - button [ref=e285] [cursor=pointer]:
                    - img [ref=e286]
              - generic [ref=e288]:
                - paragraph [ref=e289]:
                  - img [ref=e290]
                  - text: PW-Mon comment 1776755228724
                - generic [ref=e292]:
                  - button [ref=e293] [cursor=pointer]:
                    - img [ref=e294]
                  - button [ref=e296] [cursor=pointer]:
                    - img [ref=e297]
              - generic [ref=e299]:
                - paragraph [ref=e300]:
                  - img [ref=e301]
                  - text: PW-Mon comment 1776754863837
                - generic [ref=e303]:
                  - button [ref=e304] [cursor=pointer]:
                    - img [ref=e305]
                  - button [ref=e307] [cursor=pointer]:
                    - img [ref=e308]
              - generic [ref=e310]:
                - paragraph [ref=e311]:
                  - img [ref=e312]
                  - text: PW-Mon comment 1776754588075 edited
                - generic [ref=e314]:
                  - button [ref=e315] [cursor=pointer]:
                    - img [ref=e316]
                  - button [ref=e318] [cursor=pointer]:
                    - img [ref=e319]
              - generic [ref=e321]:
                - paragraph [ref=e322]:
                  - img [ref=e323]
                  - text: PW-Mon comment 1776754115504
                - generic [ref=e325]:
                  - button [ref=e326] [cursor=pointer]:
                    - img [ref=e327]
                  - button [ref=e329] [cursor=pointer]:
                    - img [ref=e330]
              - generic [ref=e332]:
                - paragraph [ref=e333]:
                  - img [ref=e334]
                  - text: PW-Mon comment 1776753123002
                - generic [ref=e336]:
                  - button [ref=e337] [cursor=pointer]:
                    - img [ref=e338]
                  - button [ref=e340] [cursor=pointer]:
                    - img [ref=e341]
              - generic [ref=e343]:
                - paragraph [ref=e344]:
                  - img [ref=e345]
                  - text: PW-Mon comment 1776751892598
                - generic [ref=e347]:
                  - button [ref=e348] [cursor=pointer]:
                    - img [ref=e349]
                  - button [ref=e351] [cursor=pointer]:
                    - img [ref=e352]
              - generic [ref=e354]:
                - paragraph [ref=e355]:
                  - img [ref=e356]
                  - text: PW-Mon comment 1776697584358
                - generic [ref=e358]:
                  - button [ref=e359] [cursor=pointer]:
                    - img [ref=e360]
                  - button [ref=e362] [cursor=pointer]:
                    - img [ref=e363]
              - generic [ref=e365]:
                - paragraph [ref=e366]:
                  - img [ref=e367]
                  - text: PW-Mon comment 1776696766450
                - generic [ref=e369]:
                  - button [ref=e370] [cursor=pointer]:
                    - img [ref=e371]
                  - button [ref=e373] [cursor=pointer]:
                    - img [ref=e374]
              - generic [ref=e376]:
                - paragraph [ref=e377]:
                  - img [ref=e378]
                  - text: PW-Mon comment 1776692724979
                - generic [ref=e380]:
                  - button [ref=e381] [cursor=pointer]:
                    - img [ref=e382]
                  - button [ref=e384] [cursor=pointer]:
                    - img [ref=e385]
          - button [ref=e389] [cursor=pointer]:
            - img [ref=e391]
            - heading [level=6] [ref=e393]: Text Message
        - tablist [ref=e398]:
          - tab [ref=e399] [cursor=pointer]: Chats
          - tab [ref=e400] [cursor=pointer]: Care Plan
          - tab [ref=e401] [cursor=pointer]: Assessment
          - tab [ref=e402] [cursor=pointer]: Tasks
          - tab [selected] [ref=e403] [cursor=pointer]: Documents
          - tab [ref=e404] [cursor=pointer]: Home Exercise
          - tab [ref=e405] [cursor=pointer]: Medical History
          - tab [ref=e406] [cursor=pointer]: Enrollments
          - tab [ref=e407] [cursor=pointer]: Care Team
          - tab [ref=e408] [cursor=pointer]: Training Library
          - tab [ref=e409] [cursor=pointer]: Billing
          - tab [ref=e410] [cursor=pointer]: Summary
        - generic [ref=e414]:
          - generic [ref=e416]:
            - generic [ref=e417] [cursor=pointer]:
              - generic [ref=e418]:
                - checkbox [ref=e419]
                - img [ref=e420]
              - generic [ref=e422]: Show Archived
            - generic [ref=e425]:
              - img [ref=e427]
              - textbox [ref=e429]:
                - /placeholder: Type here to search
              - group
            - button [ref=e430] [cursor=pointer]:
              - img [ref=e431]
              - text: Assign Document
            - button [ref=e433] [cursor=pointer]:
              - img [ref=e434]
              - text: Add Document
          - navigation [ref=e436]:
            - list [ref=e437]:
              - listitem [ref=e438]:
                - heading [level=6] [ref=e439] [cursor=pointer]: Home
              - listitem [ref=e440]: ›
              - listitem [ref=e441]:
                - heading [level=6] [ref=e442] [cursor=pointer]: Home Exercise
          - generic [ref=e446]:
            - generic [ref=e447]:
              - generic [ref=e449]: "NO"
              - generic [ref=e451]: FILE NAME
              - generic [ref=e453]: TAG
              - generic [ref=e455]: SHARED
              - generic [ref=e457]: TYPE
              - generic [ref=e459]: MODIFIED
              - generic [ref=e461]: MODIFIED BY
              - generic [ref=e463]: ACTION
            - generic [ref=e464]:
              - generic [ref=e466] [cursor=pointer]: "01"
              - generic [ref=e468] [cursor=pointer]: FHome Exercise 1778510081111
              - generic [ref=e470] [cursor=pointer]: Home Exercises
              - generic [ref=e472] [cursor=pointer]: "Yes"
              - generic [ref=e474] [cursor=pointer]: Image
              - generic [ref=e476] [cursor=pointer]: 05-11-2026
              - generic [ref=e478] [cursor=pointer]: chirag kumar
              - img [ref=e483] [cursor=pointer]
            - generic [ref=e485]:
              - generic [ref=e487] [cursor=pointer]: "02"
              - generic [ref=e489] [cursor=pointer]: FHome Exercise 1778506133330
              - generic [ref=e491] [cursor=pointer]: Home Exercises
              - generic [ref=e493] [cursor=pointer]: "Yes"
              - generic [ref=e495] [cursor=pointer]: Image
              - generic [ref=e497] [cursor=pointer]: 05-11-2026
              - generic [ref=e499] [cursor=pointer]: chirag kumar
              - img [ref=e504] [cursor=pointer]
            - generic [ref=e506]:
              - generic [ref=e508] [cursor=pointer]: "03"
              - generic [ref=e510] [cursor=pointer]: FHome Exercise 1778487294085
              - generic [ref=e512] [cursor=pointer]: Home Exercises
              - generic [ref=e514] [cursor=pointer]: "Yes"
              - generic [ref=e516] [cursor=pointer]: Image
              - generic [ref=e518] [cursor=pointer]: 05-11-2026
              - generic [ref=e520] [cursor=pointer]: chirag kumar
              - img [ref=e525] [cursor=pointer]
            - generic [ref=e527]:
              - generic [ref=e529] [cursor=pointer]: "04"
              - generic [ref=e531] [cursor=pointer]: FHome Exercise 1778245361720
              - generic [ref=e533] [cursor=pointer]: Home Exercises
              - generic [ref=e535] [cursor=pointer]: "Yes"
              - generic [ref=e537] [cursor=pointer]: Image
              - generic [ref=e539] [cursor=pointer]: 05-08-2026
              - generic [ref=e541] [cursor=pointer]: chirag kumar
              - img [ref=e546] [cursor=pointer]
            - generic [ref=e548]:
              - generic [ref=e550] [cursor=pointer]: "05"
              - generic [ref=e552] [cursor=pointer]: FHome Exercise 1776782765338
              - generic [ref=e554] [cursor=pointer]: Home Exercises
              - generic [ref=e556] [cursor=pointer]: "Yes"
              - generic [ref=e558] [cursor=pointer]: Image
              - generic [ref=e560] [cursor=pointer]: 04-21-2026
              - generic [ref=e562] [cursor=pointer]: chirag kumar
              - img [ref=e567] [cursor=pointer]
            - generic [ref=e569]:
              - generic [ref=e571] [cursor=pointer]: "06"
              - generic [ref=e573] [cursor=pointer]: FHome Exercise 1776780622339
              - generic [ref=e575] [cursor=pointer]: Home Exercises
              - generic [ref=e577] [cursor=pointer]: "Yes"
              - generic [ref=e579] [cursor=pointer]: Image
              - generic [ref=e581] [cursor=pointer]: 04-21-2026
              - generic [ref=e583] [cursor=pointer]: chirag kumar
              - img [ref=e588] [cursor=pointer]
            - generic [ref=e590]:
              - generic [ref=e592] [cursor=pointer]: "07"
              - generic [ref=e594] [cursor=pointer]: FHome Exercise 1776778466094
              - generic [ref=e596] [cursor=pointer]: Home Exercises
              - generic [ref=e598] [cursor=pointer]: "Yes"
              - generic [ref=e600] [cursor=pointer]: Image
              - generic [ref=e602] [cursor=pointer]: 04-21-2026
              - generic [ref=e604] [cursor=pointer]: chirag kumar
              - img [ref=e609] [cursor=pointer]
            - generic [ref=e611]:
              - generic [ref=e613] [cursor=pointer]: "08"
              - generic [ref=e615] [cursor=pointer]: PWDoc-Multi-1776768946013
              - generic [ref=e617] [cursor=pointer]: Home Exercises
              - generic [ref=e619] [cursor=pointer]: "Yes"
              - generic [ref=e621] [cursor=pointer]: Image
              - generic [ref=e623] [cursor=pointer]: 04-21-2026
              - generic [ref=e625] [cursor=pointer]: chirag kumar
              - img [ref=e630] [cursor=pointer]
            - generic [ref=e632]:
              - generic [ref=e634] [cursor=pointer]: "09"
              - generic [ref=e636] [cursor=pointer]: PWDoc-JPG-1776768946013
              - generic [ref=e638] [cursor=pointer]: Home Exercises
              - generic [ref=e640] [cursor=pointer]: "No"
              - generic [ref=e642] [cursor=pointer]: Image
              - generic [ref=e644] [cursor=pointer]: 04-21-2026
              - generic [ref=e646] [cursor=pointer]: chirag kumar
              - img [ref=e651] [cursor=pointer]
            - generic [ref=e653]:
              - generic [ref=e655] [cursor=pointer]: "10"
              - generic [ref=e657] [cursor=pointer]: PWDoc-Multi-1776767497790
              - generic [ref=e659] [cursor=pointer]: Home Exercises
              - generic [ref=e661] [cursor=pointer]: "Yes"
              - generic [ref=e663] [cursor=pointer]: Image
              - generic [ref=e665] [cursor=pointer]: 04-21-2026
              - generic [ref=e667] [cursor=pointer]: chirag kumar
              - img [ref=e672] [cursor=pointer]
            - generic [ref=e674]:
              - generic [ref=e676] [cursor=pointer]: "11"
              - generic [ref=e678] [cursor=pointer]: PWDoc-Multi-1776625590250
              - generic [ref=e680] [cursor=pointer]: Home Exercises
              - generic [ref=e682] [cursor=pointer]: "Yes"
              - generic [ref=e684] [cursor=pointer]: Image
              - generic [ref=e686] [cursor=pointer]: 04-19-2026
              - generic [ref=e688] [cursor=pointer]: chirag kumar
              - img [ref=e693] [cursor=pointer]
            - generic [ref=e695]:
              - generic [ref=e697] [cursor=pointer]: "12"
              - generic [ref=e699] [cursor=pointer]: PWDoc-Multi-1776624537930
              - generic [ref=e701] [cursor=pointer]: Home Exercises
              - generic [ref=e703] [cursor=pointer]: "Yes"
              - generic [ref=e705] [cursor=pointer]: Image
              - generic [ref=e707] [cursor=pointer]: 04-19-2026
              - generic [ref=e709] [cursor=pointer]: chirag kumar
              - img [ref=e714] [cursor=pointer]
            - generic [ref=e716]:
              - generic [ref=e718] [cursor=pointer]: "13"
              - generic [ref=e720] [cursor=pointer]: PWDoc-JPG-1776619758798
              - generic [ref=e722] [cursor=pointer]: Home Exercises
              - generic [ref=e724] [cursor=pointer]: "No"
              - generic [ref=e726] [cursor=pointer]: Image
              - generic [ref=e728] [cursor=pointer]: 04-19-2026
              - generic [ref=e730] [cursor=pointer]: chirag kumar
              - img [ref=e735] [cursor=pointer]
            - generic [ref=e737]:
              - generic [ref=e739] [cursor=pointer]: "14"
              - generic [ref=e741] [cursor=pointer]: PWDoc-JPG-1776619124640
              - generic [ref=e743] [cursor=pointer]: Home Exercises
              - generic [ref=e745] [cursor=pointer]: "No"
              - generic [ref=e747] [cursor=pointer]: Image
              - generic [ref=e749] [cursor=pointer]: 04-19-2026
              - generic [ref=e751] [cursor=pointer]: chirag kumar
              - img [ref=e756] [cursor=pointer]
            - generic [ref=e758]:
              - generic [ref=e760] [cursor=pointer]: "15"
              - generic [ref=e762] [cursor=pointer]: PWDoc-JPG-1776618756921
              - generic [ref=e764] [cursor=pointer]: Home Exercises
              - generic [ref=e766] [cursor=pointer]: "No"
              - generic [ref=e768] [cursor=pointer]: Image
              - generic [ref=e770] [cursor=pointer]: 04-19-2026
              - generic [ref=e772] [cursor=pointer]: chirag kumar
              - img [ref=e777] [cursor=pointer]
            - generic [ref=e779]:
              - generic [ref=e781] [cursor=pointer]: "16"
              - generic [ref=e783] [cursor=pointer]: PWDoc-JPG-1776617987730
              - generic [ref=e785] [cursor=pointer]: Home Exercises
              - generic [ref=e787] [cursor=pointer]: "No"
              - generic [ref=e789] [cursor=pointer]: Image
              - generic [ref=e791] [cursor=pointer]: 04-19-2026
              - generic [ref=e793] [cursor=pointer]: chirag kumar
              - img [ref=e798] [cursor=pointer]
            - generic [ref=e800]:
              - generic [ref=e802] [cursor=pointer]: "17"
              - generic [ref=e804] [cursor=pointer]: PWDoc-JPG-1776617458505
              - generic [ref=e806] [cursor=pointer]: Home Exercises
              - generic [ref=e808] [cursor=pointer]: "No"
              - generic [ref=e810] [cursor=pointer]: Image
              - generic [ref=e812] [cursor=pointer]: 04-19-2026
              - generic [ref=e814] [cursor=pointer]: chirag kumar
              - img [ref=e819] [cursor=pointer]
            - generic [ref=e821]:
              - generic [ref=e823] [cursor=pointer]: "18"
              - generic [ref=e825] [cursor=pointer]: FHome Exercise 1776257328479
              - generic [ref=e827] [cursor=pointer]: Home Exercises
              - generic [ref=e829] [cursor=pointer]: "Yes"
              - generic [ref=e831] [cursor=pointer]: Image
              - generic [ref=e833] [cursor=pointer]: 04-15-2026
              - generic [ref=e835] [cursor=pointer]: chirag kumar
              - img [ref=e840] [cursor=pointer]
            - generic [ref=e842]:
              - generic [ref=e844] [cursor=pointer]: "19"
              - generic [ref=e846] [cursor=pointer]: FHome Exercise 1776256229262
              - generic [ref=e848] [cursor=pointer]: Home Exercises
              - generic [ref=e850] [cursor=pointer]: "Yes"
              - generic [ref=e852] [cursor=pointer]: Image
              - generic [ref=e854] [cursor=pointer]: 04-15-2026
              - generic [ref=e856] [cursor=pointer]: chirag kumar
              - img [ref=e861] [cursor=pointer]
            - generic [ref=e863]:
              - generic [ref=e865] [cursor=pointer]: "20"
              - generic [ref=e867] [cursor=pointer]: FHome Exercise 1776248987386
              - generic [ref=e869] [cursor=pointer]: Home Exercises
              - generic [ref=e871] [cursor=pointer]: "Yes"
              - generic [ref=e873] [cursor=pointer]: Image
              - generic [ref=e875] [cursor=pointer]: 04-15-2026
              - generic [ref=e877] [cursor=pointer]: chirag kumar
              - img [ref=e882] [cursor=pointer]
            - generic [ref=e884]:
              - generic [ref=e886] [cursor=pointer]: "21"
              - generic [ref=e888] [cursor=pointer]: FHome Exercise 1776247495984
              - generic [ref=e890] [cursor=pointer]: Home Exercises
              - generic [ref=e892] [cursor=pointer]: "Yes"
              - generic [ref=e894] [cursor=pointer]: Image
              - generic [ref=e896] [cursor=pointer]: 04-15-2026
              - generic [ref=e898] [cursor=pointer]: chirag kumar
              - img [ref=e903] [cursor=pointer]
  - generic [ref=e908]:
    - generic [ref=e909]:
      - heading "UPLOAD FILE" [level=5] [ref=e912]
      - generic [ref=e913]:
        - button "Cancel" [ref=e914] [cursor=pointer]:
          - heading "Cancel" [level=6] [ref=e915]
        - button "Upload" [ref=e916] [cursor=pointer]:
          - heading "Upload" [level=6] [ref=e917]
    - generic [ref=e919]:
      - generic [ref=e920]:
        - generic [ref=e922]: Tag*
        - generic [ref=e923]:
          - combobox "Home Exercises" [ref=e924] [cursor=pointer]
          - textbox: HOME_EXERCISE
          - img
          - group
      - generic [ref=e925]:
        - generic [ref=e927]: Speciality*
        - generic [ref=e928]:
          - combobox "Cardiologist" [ref=e929] [cursor=pointer]
          - textbox: "[object Object]"
          - img
          - group
      - generic [ref=e930]:
        - generic [ref=e932]: File Name*
        - textbox "Enter Note" [active] [ref=e934]: PWDoc-JPG-1778656588525
      - generic [ref=e935]:
        - paragraph [ref=e936]: Upload Result*
        - paragraph [ref=e937]: "Upload Your File,(eg: PNG,JPEG,PDF,MP4)"
        - generic [ref=e940] [cursor=pointer]:
          - heading "Drop Here Image" [level=6] [ref=e943]:
            - img [ref=e944]
            - text: Drop Here Image
          - heading "No File Selected" [level=6] [ref=e947]
      - generic [ref=e949] [cursor=pointer]:
        - generic [ref=e950]:
          - checkbox "Share with Patient" [ref=e951]
          - img [ref=e952]
        - generic [ref=e954]: Share with Patient
      - textbox "Enter Note" [ref=e957]
      - generic [ref=e959] [cursor=pointer]:
        - generic [ref=e960]:
          - checkbox "Signature Required" [ref=e961]
          - img [ref=e962]
        - generic [ref=e964]: Signature Required
  - listbox [ref=e967]:
    - option "Acupuncturist" [ref=e968] [cursor=pointer]:
      - heading "Acupuncturist" [level=6] [ref=e969]
    - option "Addiction Specialist" [ref=e970] [cursor=pointer]:
      - heading "Addiction Specialist" [level=6] [ref=e971]
    - option "Allergist" [ref=e972] [cursor=pointer]:
      - heading "Allergist" [level=6] [ref=e973]
    - option "Anesthesiologist" [ref=e974] [cursor=pointer]:
      - heading "Anesthesiologist" [level=6] [ref=e975]
    - option "Audiologist" [ref=e976] [cursor=pointer]:
      - heading "Audiologist" [level=6] [ref=e977]
    - option "Bariatric Specialist" [ref=e978] [cursor=pointer]:
      - heading "Bariatric Specialist" [level=6] [ref=e979]
    - option "Behavioral Health & Psychiatry" [ref=e980] [cursor=pointer]:
      - heading "Behavioral Health & Psychiatry" [level=6] [ref=e981]
    - option "Behavioral Health Specialist" [ref=e982] [cursor=pointer]:
      - heading "Behavioral Health Specialist" [level=6] [ref=e983]
    - option "Breast Surgeon" [ref=e984] [cursor=pointer]:
      - heading "Breast Surgeon" [level=6] [ref=e985]
    - option "Cardiologist" [ref=e986] [cursor=pointer]:
      - heading "Cardiologist" [level=6] [ref=e987]
    - option "Cardiology" [ref=e988] [cursor=pointer]:
      - heading "Cardiology" [level=6] [ref=e989]
    - option "Cardiothoracic Surgeon" [ref=e990] [cursor=pointer]:
      - heading "Cardiothoracic Surgeon" [level=6] [ref=e991]
    - option "Child Psychologist" [ref=e992] [cursor=pointer]:
      - heading "Child Psychologist" [level=6] [ref=e993]
    - option "Chiropractic" [ref=e994] [cursor=pointer]:
      - heading "Chiropractic" [level=6] [ref=e995]
    - option "Chiropractor" [ref=e996] [cursor=pointer]:
      - heading "Chiropractor" [level=6] [ref=e997]
    - option "Colorectal Surgeon" [ref=e998] [cursor=pointer]:
      - heading "Colorectal Surgeon" [level=6] [ref=e999]
    - option "Cosmetic Surgeon" [ref=e1000] [cursor=pointer]:
      - heading "Cosmetic Surgeon" [level=6] [ref=e1001]
    - option "Dentist" [ref=e1002] [cursor=pointer]:
      - heading "Dentist" [level=6] [ref=e1003]
    - option "Dermatologist" [ref=e1004] [cursor=pointer]:
      - heading "Dermatologist" [level=6] [ref=e1005]
    - option "Dermatology" [ref=e1006] [cursor=pointer]:
      - heading "Dermatology" [level=6] [ref=e1007]
    - option "Developmental Pediatrician" [ref=e1008] [cursor=pointer]:
      - heading "Developmental Pediatrician" [level=6] [ref=e1009]
    - option "Diabetologist" [ref=e1010] [cursor=pointer]:
      - heading "Diabetologist" [level=6] [ref=e1011]
    - option "Dietitian" [ref=e1012] [cursor=pointer]:
      - heading "Dietitian" [level=6] [ref=e1013]
    - option "Ear, Nose & Throat (ENT) Specialist / Otolaryngologist" [ref=e1014] [cursor=pointer]:
      - heading "Ear, Nose & Throat (ENT) Specialist / Otolaryngologist" [level=6] [ref=e1015]
    - option "Endocrinologist" [ref=e1016] [cursor=pointer]:
      - heading "Endocrinologist" [level=6] [ref=e1017]
    - option "Endodontist" [ref=e1018] [cursor=pointer]:
      - heading "Endodontist" [level=6] [ref=e1019]
    - option "Epileptologist" [ref=e1020] [cursor=pointer]:
      - heading "Epileptologist" [level=6] [ref=e1021]
    - option "Family Physician" [ref=e1022] [cursor=pointer]:
      - heading "Family Physician" [level=6] [ref=e1023]
    - option "Foot and Ankle Specialist" [ref=e1024] [cursor=pointer]:
      - heading "Foot and Ankle Specialist" [level=6] [ref=e1025]
    - option "Gastroenterologist" [ref=e1026] [cursor=pointer]:
      - heading "Gastroenterologist" [level=6] [ref=e1027]
    - option "Gastroenterology" [ref=e1028] [cursor=pointer]:
      - heading "Gastroenterology" [level=6] [ref=e1029]
    - option "General Surgeon" [ref=e1030] [cursor=pointer]:
      - heading "General Surgeon" [level=6] [ref=e1031]
    - option "Geriatrician" [ref=e1032] [cursor=pointer]:
      - heading "Geriatrician" [level=6] [ref=e1033]
    - option "Gynecologist" [ref=e1034] [cursor=pointer]:
      - heading "Gynecologist" [level=6] [ref=e1035]
    - option "Gynecology" [ref=e1036] [cursor=pointer]:
      - heading "Gynecology" [level=6] [ref=e1037]
    - option "Hand Surgeon" [ref=e1038] [cursor=pointer]:
      - heading "Hand Surgeon" [level=6] [ref=e1039]
    - option "Head & Neck Surgeon" [ref=e1040] [cursor=pointer]:
      - heading "Head & Neck Surgeon" [level=6] [ref=e1041]
    - option "Hematologist" [ref=e1042] [cursor=pointer]:
      - heading "Hematologist" [level=6] [ref=e1043]
    - option "Hepatologist" [ref=e1044] [cursor=pointer]:
      - heading "Hepatologist" [level=6] [ref=e1045]
    - option "Homeopath / Holistic Practitioner" [ref=e1046] [cursor=pointer]:
      - heading "Homeopath / Holistic Practitioner" [level=6] [ref=e1047]
    - option "Immunologist" [ref=e1048] [cursor=pointer]:
      - heading "Immunologist" [level=6] [ref=e1049]
    - option "Infectious Disease Specialist" [ref=e1050] [cursor=pointer]:
      - heading "Infectious Disease Specialist" [level=6] [ref=e1051]
    - option "Infertility Specialist" [ref=e1052] [cursor=pointer]:
      - heading "Infertility Specialist" [level=6] [ref=e1053]
    - option "Internal Medicine" [ref=e1054] [cursor=pointer]:
      - heading "Internal Medicine" [level=6] [ref=e1055]
    - option "Internal Medicine Physician" [ref=e1056] [cursor=pointer]:
      - heading "Internal Medicine Physician" [level=6] [ref=e1057]
    - option "Naturopath" [ref=e1058] [cursor=pointer]:
      - heading "Naturopath" [level=6] [ref=e1059]
    - option "Neonatologist" [ref=e1060] [cursor=pointer]:
      - heading "Neonatologist" [level=6] [ref=e1061]
    - option "Nephrologist" [ref=e1062] [cursor=pointer]:
      - heading "Nephrologist" [level=6] [ref=e1063]
    - option "Neurologist" [ref=e1064] [cursor=pointer]:
      - heading "Neurologist" [level=6] [ref=e1065]
    - option "Neurology" [ref=e1066] [cursor=pointer]:
      - heading "Neurology" [level=6] [ref=e1067]
    - option "Neurosurgeon" [ref=e1068] [cursor=pointer]:
      - heading "Neurosurgeon" [level=6] [ref=e1069]
    - option "Nuclear Medicine Physician" [ref=e1070] [cursor=pointer]:
      - heading "Nuclear Medicine Physician" [level=6] [ref=e1071]
    - option "Nurse Practitioner" [ref=e1072] [cursor=pointer]:
      - heading "Nurse Practitioner" [level=6] [ref=e1073]
    - option "Nutritionist" [ref=e1074] [cursor=pointer]:
      - heading "Nutritionist" [level=6] [ref=e1075]
    - option "Obstetrician & Gynecologist" [ref=e1076] [cursor=pointer]:
      - heading "Obstetrician & Gynecologist" [level=6] [ref=e1077]
    - option "Occupational Medicine Physician" [ref=e1078] [cursor=pointer]:
      - heading "Occupational Medicine Physician" [level=6] [ref=e1079]
    - option "Oncologist" [ref=e1080] [cursor=pointer]:
      - heading "Oncologist" [level=6] [ref=e1081]
    - option "Oncology" [ref=e1082] [cursor=pointer]:
      - heading "Oncology" [level=6] [ref=e1083]
    - option "Ophthalmologist" [ref=e1084] [cursor=pointer]:
      - heading "Ophthalmologist" [level=6] [ref=e1085]
    - option "Ophthalmology" [ref=e1086] [cursor=pointer]:
      - heading "Ophthalmology" [level=6] [ref=e1087]
    - option "Optometrist" [ref=e1088] [cursor=pointer]:
      - heading "Optometrist" [level=6] [ref=e1089]
    - option "Oral & Maxillofacial Surgeon" [ref=e1090] [cursor=pointer]:
      - heading "Oral & Maxillofacial Surgeon" [level=6] [ref=e1091]
    - option "Orthodontist" [ref=e1092] [cursor=pointer]:
      - heading "Orthodontist" [level=6] [ref=e1093]
    - option "Orthopedics" [ref=e1094] [cursor=pointer]:
      - heading "Orthopedics" [level=6] [ref=e1095]
    - option "Orthopedic Surgeon" [ref=e1096] [cursor=pointer]:
      - heading "Orthopedic Surgeon" [level=6] [ref=e1097]
    - option "Osteopathic Physician" [ref=e1098] [cursor=pointer]:
      - heading "Osteopathic Physician" [level=6] [ref=e1099]
    - option "Pain Management" [ref=e1100] [cursor=pointer]:
      - heading "Pain Management" [level=6] [ref=e1101]
    - option "Pain Management Specialist" [ref=e1102] [cursor=pointer]:
      - heading "Pain Management Specialist" [level=6] [ref=e1103]
    - option "Palliative Care Physician" [ref=e1104] [cursor=pointer]:
      - heading "Palliative Care Physician" [level=6] [ref=e1105]
    - option "Pathologist" [ref=e1106] [cursor=pointer]:
      - heading "Pathologist" [level=6] [ref=e1107]
    - option "Pediatrician" [ref=e1108] [cursor=pointer]:
      - heading "Pediatrician" [level=6] [ref=e1109]
    - option "Pediatrics" [ref=e1110] [cursor=pointer]:
      - heading "Pediatrics" [level=6] [ref=e1111]
    - option "Pedodontist" [ref=e1112] [cursor=pointer]:
      - heading "Pedodontist" [level=6] [ref=e1113]
    - option "Periodontist" [ref=e1114] [cursor=pointer]:
      - heading "Periodontist" [level=6] [ref=e1115]
    - option "Physical Medicine & Rehabilitation Specialist" [ref=e1116] [cursor=pointer]:
      - heading "Physical Medicine & Rehabilitation Specialist" [level=6] [ref=e1117]
    - option "Physical Therapy" [ref=e1118] [cursor=pointer]:
      - heading "Physical Therapy" [level=6] [ref=e1119]
    - option "Physiotherapist" [ref=e1120] [cursor=pointer]:
      - heading "Physiotherapist" [level=6] [ref=e1121]
    - option "Plastic Surgeon" [ref=e1122] [cursor=pointer]:
      - heading "Plastic Surgeon" [level=6] [ref=e1123]
    - option "Podiatrist" [ref=e1124] [cursor=pointer]:
      - heading "Podiatrist" [level=6] [ref=e1125]
    - option "Podiatry" [ref=e1126] [cursor=pointer]:
      - heading "Podiatry" [level=6] [ref=e1127]
    - option "Primary Care" [ref=e1128] [cursor=pointer]:
      - heading "Primary Care" [level=6] [ref=e1129]
    - option "Primary Care Physician" [ref=e1130] [cursor=pointer]:
      - heading "Primary Care Physician" [level=6] [ref=e1131]
    - option "Prosthodontist" [ref=e1132] [cursor=pointer]:
      - heading "Prosthodontist" [level=6] [ref=e1133]
    - option "Psychiatrist" [ref=e1134] [cursor=pointer]:
      - heading "Psychiatrist" [level=6] [ref=e1135]
    - option "Psychologist" [ref=e1136] [cursor=pointer]:
      - heading "Psychologist" [level=6] [ref=e1137]
    - option "Pulmonologist" [ref=e1138] [cursor=pointer]:
      - heading "Pulmonologist" [level=6] [ref=e1139]
    - option "Radiation Oncologist" [ref=e1140] [cursor=pointer]:
      - heading "Radiation Oncologist" [level=6] [ref=e1141]
    - option "Reconstructive Orthopedic Surgeon" [ref=e1142] [cursor=pointer]:
      - heading "Reconstructive Orthopedic Surgeon" [level=6] [ref=e1143]
    - option "Reproductive Endocrinologist" [ref=e1144] [cursor=pointer]:
      - heading "Reproductive Endocrinologist" [level=6] [ref=e1145]
    - option "Rheumatologist" [ref=e1146] [cursor=pointer]:
      - heading "Rheumatologist" [level=6] [ref=e1147]
    - option "Sleep Medicine Specialist" [ref=e1148] [cursor=pointer]:
      - heading "Sleep Medicine Specialist" [level=6] [ref=e1149]
    - option "Speech and Language Pathologist" [ref=e1150] [cursor=pointer]:
      - heading "Speech and Language Pathologist" [level=6] [ref=e1151]
    - option "Spine Surgeon" [ref=e1152] [cursor=pointer]:
      - heading "Spine Surgeon" [level=6] [ref=e1153]
    - option "Sports Medicine Specialist" [ref=e1154] [cursor=pointer]:
      - heading "Sports Medicine Specialist" [level=6] [ref=e1155]
    - option "Therapist / Counselor" [ref=e1156] [cursor=pointer]:
      - heading "Therapist / Counselor" [level=6] [ref=e1157]
    - option "Thoracic Surgeon" [ref=e1158] [cursor=pointer]:
      - heading "Thoracic Surgeon" [level=6] [ref=e1159]
    - option "Transplant Surgeon" [ref=e1160] [cursor=pointer]:
      - heading "Transplant Surgeon" [level=6] [ref=e1161]
    - option "Urgent Care" [ref=e1162] [cursor=pointer]:
      - heading "Urgent Care" [level=6] [ref=e1163]
    - option "Urgent Care Specialist" [ref=e1164] [cursor=pointer]:
      - heading "Urgent Care Specialist" [level=6] [ref=e1165]
    - option "Urogynecologist" [ref=e1166] [cursor=pointer]:
      - heading "Urogynecologist" [level=6] [ref=e1167]
    - option "Urologist" [ref=e1168] [cursor=pointer]:
      - heading "Urologist" [level=6] [ref=e1169]
    - option "Urology" [ref=e1170] [cursor=pointer]:
      - heading "Urology" [level=6] [ref=e1171]
    - option "Vascular Surgeon" [ref=e1172] [cursor=pointer]:
      - heading "Vascular Surgeon" [level=6] [ref=e1173]
```

# Test source

```ts
  40  |         await page.locator("button:has-text('CCM')").first().click();
  41  |         await page.waitForLoadState('networkidle');
  42  |         await settle(page, 2000);
  43  |         await page.getByRole('tab', { name: 'Documents', exact: true }).click();
  44  |         await settle(page, 2500);
  45  |         Logger.info('Setup ✓: on patient-chart CCM → Documents');
  46  | 
  47  |         // =====================================================================
  48  |         // HELPERS (scoped to patient-chart Documents tab)
  49  |         // =====================================================================
  50  |         const folders = ['Home Exercise', 'Education', 'Challenges', 'Care Plan', 'Consent'];
  51  |         const folderToTag: Record<string, string> = {
  52  |             'Home Exercise': 'Home Exercises',
  53  |             'Education': 'Education',
  54  |             'Challenges': 'Challenges',
  55  |             'Care Plan': 'Care Plan',
  56  |             'Consent': 'Consent',
  57  |         };
  58  | 
  59  |         const openFolder = async (name: string): Promise<boolean> => {
  60  |             const folderEl = page.locator(
  61  |                 `//h6[normalize-space()='${name}'] | //span[normalize-space()='${name}'] | //p[normalize-space()='${name}']`
  62  |             ).first();
  63  |             if (!(await folderEl.isVisible({ timeout: 5000 }).catch(() => false))) return false;
  64  |             await folderEl.click();
  65  |             await page.waitForLoadState('networkidle');
  66  |             await settle(page, 1500);
  67  |             return true;
  68  |         };
  69  | 
  70  |         const goBackToDocumentsRoot = async (): Promise<void> => {
  71  |             // Prefer breadcrumb "Home"; fall back to re-clicking the Documents tab.
  72  |             const homeCrumb = page.getByRole('heading', { name: /^Home$/ }).first();
  73  |             if (await homeCrumb.isVisible({ timeout: 2000 }).catch(() => false)) {
  74  |                 await homeCrumb.click();
  75  |             } else {
  76  |                 await page.getByRole('tab', { name: 'Documents', exact: true }).click();
  77  |             }
  78  |             await page.waitForLoadState('networkidle');
  79  |             await settle(page, 1500);
  80  |         };
  81  | 
  82  |         const uploadDocument = async (opts: {
  83  |             folder: string;
  84  |             fileName: string;
  85  |             filePath: string;
  86  |             tag?: string;
  87  |             speciality?: string;
  88  |             description?: string;
  89  |             signatureRequired?: boolean;
  90  |             notes?: string;
  91  |             shareWithPatientName?: string;
  92  |         }): Promise<void> => {
  93  |             Logger.step(`Uploading "${opts.fileName}" to "${opts.folder}"`);
  94  |             await goBackToDocumentsRoot();
  95  |             const opened = await openFolder(opts.folder);
  96  |             expect(opened, `Folder "${opts.folder}" should be accessible`).toBeTruthy();
  97  | 
  98  |             // Chart context uses "Add Document" (the global Document Library uses "Upload Material").
  99  |             const addBtn = page.getByRole('button', { name: /Add Document|Upload Material/i }).first();
  100 |             await addBtn.waitFor({ state: 'visible', timeout: 10000 });
  101 |             await addBtn.click();
  102 |             await settle(page, 2000);
  103 | 
  104 |             // Drawer structure (chart context):
  105 |             //   Tag*        → combobox "Select"
  106 |             //   Speciality* → combobox "Select"
  107 |             //   File Name*  → textbox (placeholder "Enter Note", label "File Name*")
  108 |             //   Upload Result* → file drop zone
  109 |             //   "Share with Patient" checkbox
  110 |             //   button <h6>Upload</h6>
  111 | 
  112 |             // Tag
  113 |             const tag = opts.tag ?? folderToTag[opts.folder];
  114 |             const tagCombo = page.locator("xpath=//*[normalize-space()='Tag*']/following::*[@role='combobox'][1]").first();
  115 |             await tagCombo.waitFor({ state: 'visible', timeout: 10000 });
  116 |             await tagCombo.click();
  117 |             await settle(page, 1000);
  118 |             await page.getByRole('option', { name: tag, exact: false }).first().click();
  119 |             await settle(page, 500);
  120 | 
  121 |             // Speciality
  122 |             const speciality = opts.speciality ?? 'Cardiologist';
  123 |             const specCombo = page.locator("xpath=//*[normalize-space()='Speciality*']/following::*[@role='combobox'][1]").first();
  124 |             await specCombo.waitFor({ state: 'visible', timeout: 10000 });
  125 |             await specCombo.click();
  126 |             await settle(page, 1000);
  127 |             await page.getByRole('option', { name: speciality, exact: false }).first().click();
  128 |             await settle(page, 500);
  129 | 
  130 |             // File Name (labeled "File Name*", but its input's placeholder is "Enter Note").
  131 |             const fileNameInput = page.locator(
  132 |                 "xpath=//*[normalize-space()='File Name*']/following::input[1]"
  133 |             ).first();
  134 |             await fileNameInput.fill(opts.fileName);
  135 |             await settle(page, 300);
  136 | 
  137 |             // File upload — the drop zone has a hidden <input type='file'>. The server
  138 |             // upload runs async; we MUST wait for it to complete before clicking Upload,
  139 |             // otherwise the backend returns "File key is missing" on submit.
> 140 |             await page.locator("input[type='file']").first().setInputFiles(opts.filePath);
      |             ^ Error: ENOENT: no such file or directory, stat 'C:/Users/TTPL-LNVE16-0380/Desktop/Docs/4mb.jpg'
  141 | 
  142 |             // (a) Wait for progressbar (if any) to hide.
  143 |             await page.locator("[role='progressbar']").waitFor({ state: 'hidden', timeout: 120000 }).catch(() => {});
  144 | 
  145 |             // (b) Wait for the "Uploaded Preview" affordance OR an inline file-name
  146 |             // chip to appear — either indicates the server confirmed the upload.
  147 |             const uploadSignal = page.locator(
  148 |                 "img[alt='Uploaded Preview'], img[alt*='Preview'], [data-testid*='upload-success' i]"
  149 |             ).first();
  150 |             await uploadSignal
  151 |                 .waitFor({ state: 'visible', timeout: 60000 })
  152 |                 .catch(() => Logger.info('No upload-success signal — may be a non-image asset; relying on network idle'));
  153 | 
  154 |             // (c) Settle for any pending network roundtrip. SPA has background polling
  155 |             // that prevents `networkidle` from ever firing — use a fixed settle instead.
  156 |             await settle(page, 4000);
  157 | 
  158 |             // Description (optional)
  159 |             if (opts.description) {
  160 |                 const descInput = page.getByPlaceholder(/Description|Enter Description/i).first();
  161 |                 if (await descInput.isVisible({ timeout: 2000 }).catch(() => false)) {
  162 |                     await descInput.fill(opts.description);
  163 |                 }
  164 |             }
  165 | 
  166 |             // "Share with Patient" is a checkbox. For multi-patient share scenarios we
  167 |             // toggle it on (patient pre-association comes from the active patient chart
  168 |             // context, so no separate patient picker is exposed in most variants).
  169 |             if (opts.shareWithPatientName) {
  170 |                 const shareCheckbox = page.getByRole('checkbox', { name: /Share with Patient/i }).first();
  171 |                 if (await shareCheckbox.isVisible({ timeout: 3000 }).catch(() => false)) {
  172 |                     await shareCheckbox.check({ force: true }).catch(() => shareCheckbox.click({ force: true }));
  173 |                     await settle(page, 800);
  174 |                 }
  175 |             }
  176 | 
  177 |             // Wait for async enable handlers to finish.
  178 |             await page.waitForFunction(() => {
  179 |                 const btns = Array.from(document.querySelectorAll('button'));
  180 |                 return btns.some(b => !b.disabled && b.getAttribute('aria-label') === null &&
  181 |                     !!b.querySelector('h6')?.textContent?.match(/^Upload$/));
  182 |             }, { timeout: 120000 });
  183 |             await settle(page, 2000);
  184 | 
  185 |             // Upload button — accessible name "Upload", exact match. This is the drawer's
  186 |             // submit button (distinct from the drawer title "UPLOAD FILE").
  187 |             const uploadBtn = page.getByRole('button', { name: 'Upload', exact: true });
  188 |             await uploadBtn.scrollIntoViewIfNeeded().catch(() => {});
  189 |             await uploadBtn.click();
  190 | 
  191 |             // Wait for the drawer to close — watch the drawer title "UPLOAD FILE" specifically.
  192 |             const drawerTitle = page.getByRole('heading', { name: 'UPLOAD FILE', exact: true });
  193 |             const closed = await drawerTitle.waitFor({ state: 'hidden', timeout: 60000 })
  194 |                 .then(() => true)
  195 |                 .catch(() => false);
  196 |             if (!closed) {
  197 |                 Logger.info('Upload drawer did not close on first click — retrying');
  198 |                 await uploadBtn.click({ force: true }).catch(() => {});
  199 |                 await drawerTitle.waitFor({ state: 'hidden', timeout: 60000 }).catch(() => {});
  200 |             }
  201 |             await settle(page, 1500);
  202 |             Logger.info(`Uploaded "${opts.fileName}" to "${opts.folder}"`);
  203 |         };
  204 | 
  205 |         const openDocumentActionMenu = async (fileName: string): Promise<void> => {
  206 |             await page.keyboard.press('Escape').catch(() => {});
  207 |             await settle(page, 200);
  208 |             const cell = page.getByText(fileName, { exact: true }).first();
  209 |             await cell.waitFor({ state: 'visible', timeout: 10000 });
  210 |             const row = cell.locator("xpath=./ancestor::*[.//*[@data-testid='MoreVertIcon']][1]");
  211 |             await row.locator("[data-testid='MoreVertIcon']").last().click();
  212 |             await settle(page, 1000);
  213 |         };
  214 | 
  215 |         const clickRowAction = async (fileName: string, action: RegExp): Promise<void> => {
  216 |             await openDocumentActionMenu(fileName);
  217 |             const actionBtn = page.getByRole('button', { name: action }).last();
  218 |             if (await actionBtn.isVisible({ timeout: 3000 }).catch(() => false)) {
  219 |                 await actionBtn.click();
  220 |             } else {
  221 |                 await page.getByRole('menuitem', { name: action }).first().click();
  222 |             }
  223 |             await settle(page, 1500);
  224 |         };
  225 | 
  226 |         const createdDocs: string[] = [];
  227 | 
  228 |         // =====================================================================
  229 |         // SCENARIO 1 + 3 — Folders visible and accessible
  230 |         // =====================================================================
  231 |         await test.step('Scenarios 1 + 3: View Documents tab — all folders visible and accessible', async () => {
  232 |             await goBackToDocumentsRoot();
  233 |             const docsText = await page.locator('main').innerText();
  234 |             for (const f of folders) {
  235 |                 expect(docsText, `Documents landing must show "${f}" folder`)
  236 |                     .toMatch(new RegExp(f.replace(/ /g, '\\s*'), 'i'));
  237 |             }
  238 |             Logger.info(`Scenario 1 ✓: root shows all ${folders.length} folders`);
  239 | 
  240 |             // Navigate into each folder and back out to verify access.
```