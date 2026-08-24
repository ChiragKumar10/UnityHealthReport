# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: provider-portal/enrollment/enrollment-care-plan-vital-threshold-triggers-alert.spec.ts >> Care Plan vital threshold triggers alert on out-of-range readings >> Reading below Min and above Max each generate an alert for the patient
- Location: tests/web/provider-portal/enrollment/enrollment-care-plan-vital-threshold-triggers-alert.spec.ts:44:9

# Error details

```
TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
Call log:
  - waiting for locator('//h5[text()="NEW ENROLLMENT"]') to be visible

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
      - generic [ref=f1e228]:
        - tablist [ref=f1e231]:
          - tab [ref=f1e232] [cursor=pointer]:
            - generic [ref=f1e233]:
              - generic [ref=f1e234]: RPM
              - button [ref=f1e235]
          - tab [selected] [ref=f1e238] [cursor=pointer]:
            - generic [ref=f1e239]:
              - generic [ref=f1e240]: RTM
              - button [ref=f1e241]
          - tab [ref=f1e244] [cursor=pointer]:
            - generic [ref=f1e245]:
              - generic [ref=f1e246]: CCM
              - button [ref=f1e247]
          - tab [ref=f1e250] [cursor=pointer]:
            - generic [ref=f1e251]:
              - generic [ref=f1e252]: PCM
              - button [ref=f1e253]
        - generic [ref=f1e257]:
          - generic [ref=f1e259]:
            - paragraph [ref=f1e261]: Enrollments
            - table [ref=f1e263]:
              - rowgroup [ref=f1e264]:
                - row [ref=f1e265]:
                  - cell [ref=f1e266]:
                    - paragraph [ref=f1e267] [cursor=pointer]: Requests
                  - cell [ref=f1e268]:
                    - paragraph [ref=f1e269] [cursor=pointer]: "0"
                - row [ref=f1e270]:
                  - cell [ref=f1e271]:
                    - paragraph [ref=f1e272] [cursor=pointer]: New
                  - cell [ref=f1e273]:
                    - paragraph [ref=f1e274] [cursor=pointer]: "27"
                - row [ref=f1e275]:
                  - cell [ref=f1e276]:
                    - paragraph [ref=f1e277] [cursor=pointer]: Active
                  - cell [ref=f1e278]:
                    - paragraph [ref=f1e279] [cursor=pointer]: "566"
                - row [ref=f1e280]:
                  - cell [ref=f1e281]:
                    - paragraph [ref=f1e282] [cursor=pointer]: Closed
                  - cell [ref=f1e283]:
                    - paragraph [ref=f1e284] [cursor=pointer]: "69"
          - generic [ref=f1e286]:
            - paragraph [ref=f1e288]: Monitoring
            - table [ref=f1e290]:
              - rowgroup [ref=f1e291]:
                - row [ref=f1e292]:
                  - cell [ref=f1e293]:
                    - paragraph [ref=f1e294] [cursor=pointer]: 0 Alerts
                  - cell [ref=f1e295]:
                    - paragraph [ref=f1e296] [cursor=pointer]: 0 Resolved
                  - cell [ref=f1e297]:
                    - paragraph [ref=f1e298] [cursor=pointer]: 0 Not Resolved
                - row [ref=f1e299]:
                  - cell [ref=f1e300]:
                    - paragraph [ref=f1e301] [cursor=pointer]: 549 No Data
                  - cell [ref=f1e302]:
                    - paragraph [ref=f1e303] [cursor=pointer]: 0 Complete
                  - cell [ref=f1e304]:
                    - paragraph [ref=f1e305] [cursor=pointer]: 549 Not Complete
                - row [ref=f1e306]:
                  - cell [ref=f1e307]:
                    - paragraph [ref=f1e308] [cursor=pointer]: 0 Data
                  - cell [ref=f1e309]:
                    - paragraph [ref=f1e310] [cursor=pointer]: 0 Reviewed
                  - cell [ref=f1e311]:
                    - paragraph [ref=f1e312] [cursor=pointer]: 0 Unreviewed
          - generic [ref=f1e314]:
            - paragraph [ref=f1e316]: Interaction
            - table [ref=f1e318]:
              - rowgroup [ref=f1e319]:
                - row [ref=f1e320]:
                  - cell [ref=f1e321]:
                    - paragraph [ref=f1e322] [cursor=pointer]: Week 1
                  - cell [ref=f1e323]:
                    - paragraph [ref=f1e324] [cursor=pointer]: "17"
                - row [ref=f1e325]:
                  - cell [ref=f1e326]:
                    - paragraph [ref=f1e327] [cursor=pointer]: Week 2
                  - cell [ref=f1e328]:
                    - paragraph [ref=f1e329] [cursor=pointer]: "0"
                - row [ref=f1e330]:
                  - cell [ref=f1e331]:
                    - paragraph [ref=f1e332] [cursor=pointer]: Week 3
                  - cell [ref=f1e333]:
                    - paragraph [ref=f1e334] [cursor=pointer]: "0"
                - row [ref=f1e335]:
                  - cell [ref=f1e336]:
                    - paragraph [ref=f1e337] [cursor=pointer]: Week 4
                  - cell [ref=f1e338]:
                    - paragraph [ref=f1e339] [cursor=pointer]: "549"
        - generic [ref=f1e343]:
          - generic [ref=f1e344]:
            - heading [level=5] [ref=f1e345]: ENROLLMENTS (NEW-RTM)
            - generic [ref=f1e346]:
              - generic [ref=f1e351]:
                - combobox [ref=f1e352]
                - button [ref=f1e354] [cursor=pointer]
                - group
              - generic [ref=f1e358] [cursor=pointer]:
                - checkbox [ref=f1e360]
                - generic [ref=f1e363]: SelfPay
              - generic [ref=f1e364]:
                - generic [ref=f1e367]:
                  - textbox [ref=f1e371]:
                    - /placeholder: Search by Patient Name
                  - group
                - generic [ref=f1e376]:
                  - combobox [ref=f1e377]: All Provider
                  - button [ref=f1e379] [cursor=pointer]
                  - group
                - generic [ref=f1e386]:
                  - combobox [ref=f1e387]: All Care Manager
                  - button [ref=f1e389] [cursor=pointer]
                  - group
          - generic [ref=f1e394]:
            - generic [ref=f1e395]:
              - checkbox [ref=f1e398] [cursor=pointer]
              - generic [ref=f1e401] [cursor=pointer]: NAME ▲
              - generic [ref=f1e403]: CONTACT NUMBER
              - generic [ref=f1e405]: DATE ADDED
              - generic [ref=f1e407]: INSURANCE NAME
              - generic [ref=f1e409]: CONSENT
              - generic [ref=f1e411]: INSURANCE
              - generic [ref=f1e413]: CONDITIONS
              - generic [ref=f1e415]: INTRODUCTION
              - generic [ref=f1e417]: EDUCATION
              - generic [ref=f1e419]: ACTION
            - generic [ref=f1e421]:
              - checkbox [ref=f1e424] [cursor=pointer]
              - generic [ref=f1e427]: Stroman, Vivian
              - generic [ref=f1e429]: 877-892-2650
              - generic [ref=f1e431]: 08-24-2026
              - generic [ref=f1e433]: SelfPay
              - checkbox [ref=f1e438] [cursor=pointer]
              - checkbox [checked] [ref=f1e444] [cursor=pointer]
              - checkbox [checked] [ref=f1e450] [cursor=pointer]
              - checkbox [ref=f1e456] [cursor=pointer]
              - checkbox [ref=f1e462] [cursor=pointer]
              - generic [ref=f1e468] [cursor=pointer]
            - generic [ref=f1e471]:
              - checkbox [ref=f1e474] [cursor=pointer]
              - generic [ref=f1e477]: Dibbert, Carson
              - generic [ref=f1e479]: 715-011-8166
              - generic [ref=f1e481]: 08-24-2026
              - generic [ref=f1e483]: SelfPay
              - checkbox [ref=f1e488] [cursor=pointer]
              - checkbox [checked] [ref=f1e494] [cursor=pointer]
              - checkbox [checked] [ref=f1e500] [cursor=pointer]
              - checkbox [ref=f1e506] [cursor=pointer]
              - checkbox [ref=f1e512] [cursor=pointer]
              - generic [ref=f1e518] [cursor=pointer]
            - generic [ref=f1e521]:
              - checkbox [ref=f1e524] [cursor=pointer]
              - generic [ref=f1e527]: Murazik, Kiera
              - generic [ref=f1e529]: 937-529-1530
              - generic [ref=f1e531]: 08-24-2026
              - generic [ref=f1e533]: SelfPay
              - checkbox [ref=f1e538] [cursor=pointer]
              - checkbox [checked] [ref=f1e544] [cursor=pointer]
              - checkbox [checked] [ref=f1e550] [cursor=pointer]
              - checkbox [ref=f1e556] [cursor=pointer]
              - checkbox [ref=f1e562] [cursor=pointer]
              - generic [ref=f1e568] [cursor=pointer]
            - generic [ref=f1e571]:
              - checkbox [ref=f1e574] [cursor=pointer]
              - generic [ref=f1e577]: Oberbrunner, Vito
              - generic [ref=f1e579]: 690-013-3617
              - generic [ref=f1e581]: 08-24-2026
              - generic [ref=f1e583]: SelfPay
              - checkbox [ref=f1e588] [cursor=pointer]
              - checkbox [checked] [ref=f1e594] [cursor=pointer]
              - checkbox [checked] [ref=f1e600] [cursor=pointer]
              - checkbox [ref=f1e606] [cursor=pointer]
              - checkbox [ref=f1e612] [cursor=pointer]
              - generic [ref=f1e618] [cursor=pointer]
            - generic [ref=f1e621]:
              - checkbox [ref=f1e624] [cursor=pointer]
              - generic [ref=f1e627]: Champlin, Maryam
              - generic [ref=f1e629]: 620-138-1470
              - generic [ref=f1e631]: 08-24-2026
              - generic [ref=f1e633]: SelfPay
              - checkbox [ref=f1e638] [cursor=pointer]
              - checkbox [checked] [ref=f1e644] [cursor=pointer]
              - checkbox [checked] [ref=f1e650] [cursor=pointer]
              - checkbox [ref=f1e656] [cursor=pointer]
              - checkbox [ref=f1e662] [cursor=pointer]
              - generic [ref=f1e668] [cursor=pointer]
            - generic [ref=f1e671]:
              - checkbox [ref=f1e674] [cursor=pointer]
              - generic [ref=f1e677]: Ullrich, Becky
              - generic [ref=f1e679]: 997-941-7314
              - generic [ref=f1e681]: 08-24-2026
              - generic [ref=f1e683]: SelfPay
              - checkbox [ref=f1e688] [cursor=pointer]
              - checkbox [checked] [ref=f1e694] [cursor=pointer]
              - checkbox [checked] [ref=f1e700] [cursor=pointer]
              - checkbox [ref=f1e706] [cursor=pointer]
              - checkbox [ref=f1e712] [cursor=pointer]
              - generic [ref=f1e718] [cursor=pointer]
            - generic [ref=f1e721]:
              - checkbox [ref=f1e724] [cursor=pointer]
              - generic [ref=f1e727]: Ankunding, Sidney
              - generic [ref=f1e729]: 926-486-3309
              - generic [ref=f1e731]: 08-19-2026
              - generic [ref=f1e733]: SelfPay
              - checkbox [ref=f1e738] [cursor=pointer]
              - checkbox [checked] [ref=f1e744] [cursor=pointer]
              - checkbox [checked] [ref=f1e750] [cursor=pointer]
              - checkbox [checked] [ref=f1e756] [cursor=pointer]
              - checkbox [ref=f1e762] [cursor=pointer]
              - generic [ref=f1e768] [cursor=pointer]
            - generic [ref=f1e771]:
              - checkbox [ref=f1e774] [cursor=pointer]
              - generic [ref=f1e777]: Zemlak, Andreane
              - generic [ref=f1e779]: 941-400-5354
              - generic [ref=f1e781]: 08-24-2026
              - generic [ref=f1e783]: SelfPay
              - checkbox [ref=f1e788] [cursor=pointer]
              - checkbox [checked] [ref=f1e794] [cursor=pointer]
              - checkbox [checked] [ref=f1e800] [cursor=pointer]
              - checkbox [ref=f1e806] [cursor=pointer]
              - checkbox [ref=f1e812] [cursor=pointer]
              - generic [ref=f1e818] [cursor=pointer]
            - generic [ref=f1e821]:
              - checkbox [ref=f1e824] [cursor=pointer]
              - generic [ref=f1e827]: King, Angelina
              - generic [ref=f1e829]: 917-643-3636
              - generic [ref=f1e831]: 08-21-2026
              - generic [ref=f1e833]: SelfPay
              - checkbox [ref=f1e838] [cursor=pointer]
              - checkbox [checked] [ref=f1e844] [cursor=pointer]
              - checkbox [checked] [ref=f1e850] [cursor=pointer]
              - checkbox [ref=f1e856] [cursor=pointer]
              - checkbox [ref=f1e862] [cursor=pointer]
              - generic [ref=f1e868] [cursor=pointer]
            - generic [ref=f1e871]:
              - checkbox [ref=f1e874] [cursor=pointer]
              - generic [ref=f1e877]: Bogisich, Kendra
              - generic [ref=f1e879]: 642-874-8272
              - generic [ref=f1e881]: 08-21-2026
              - generic [ref=f1e883]: SelfPay
              - checkbox [ref=f1e888] [cursor=pointer]
              - checkbox [checked] [ref=f1e894] [cursor=pointer]
              - checkbox [checked] [ref=f1e900] [cursor=pointer]
              - checkbox [ref=f1e906] [cursor=pointer]
              - checkbox [ref=f1e912] [cursor=pointer]
              - generic [ref=f1e918] [cursor=pointer]
            - generic [ref=f1e921]:
              - checkbox [ref=f1e924] [cursor=pointer]
              - generic [ref=f1e927]: Cruickshank, Kristen
              - generic [ref=f1e929]: 775-025-4515
              - generic [ref=f1e931]: 08-19-2026
              - generic [ref=f1e933]: SelfPay
              - checkbox [ref=f1e938] [cursor=pointer]
              - checkbox [checked] [ref=f1e944] [cursor=pointer]
              - checkbox [checked] [ref=f1e950] [cursor=pointer]
              - checkbox [checked] [ref=f1e956] [cursor=pointer]
              - checkbox [ref=f1e962] [cursor=pointer]
              - generic [ref=f1e968] [cursor=pointer]
            - generic [ref=f1e971]:
              - checkbox [ref=f1e974] [cursor=pointer]
              - generic [ref=f1e977]: Wunsch, Todd
              - generic [ref=f1e979]: 783-124-3838
              - generic [ref=f1e981]: 08-19-2026
              - generic [ref=f1e983]: SelfPay
              - checkbox [ref=f1e988] [cursor=pointer]
              - checkbox [checked] [ref=f1e994] [cursor=pointer]
              - checkbox [checked] [ref=f1e1000] [cursor=pointer]
              - checkbox [ref=f1e1006] [cursor=pointer]
              - checkbox [ref=f1e1012] [cursor=pointer]
              - generic [ref=f1e1018] [cursor=pointer]
            - generic [ref=f1e1021]:
              - checkbox [ref=f1e1024] [cursor=pointer]
              - generic [ref=f1e1027]: Schowalter, Emelia
              - generic [ref=f1e1029]: 770-523-5512
              - generic [ref=f1e1031]: 08-19-2026
              - generic [ref=f1e1033]: SelfPay
              - checkbox [ref=f1e1038] [cursor=pointer]
              - checkbox [checked] [ref=f1e1044] [cursor=pointer]
              - checkbox [checked] [ref=f1e1050] [cursor=pointer]
              - checkbox [ref=f1e1056] [cursor=pointer]
              - checkbox [ref=f1e1062] [cursor=pointer]
              - generic [ref=f1e1068] [cursor=pointer]
            - generic [ref=f1e1071]:
              - checkbox [ref=f1e1074] [cursor=pointer]
              - generic [ref=f1e1077]: Bins, Edmond
              - generic [ref=f1e1079]: 885-100-0422
              - generic [ref=f1e1081]: 08-19-2026
              - generic [ref=f1e1083]: SelfPay
              - checkbox [ref=f1e1088] [cursor=pointer]
              - checkbox [checked] [ref=f1e1094] [cursor=pointer]
              - checkbox [checked] [ref=f1e1100] [cursor=pointer]
              - checkbox [checked] [ref=f1e1106] [cursor=pointer]
              - checkbox [ref=f1e1112] [cursor=pointer]
              - generic [ref=f1e1118] [cursor=pointer]
            - generic [ref=f1e1121]:
              - checkbox [ref=f1e1124] [cursor=pointer]
              - generic [ref=f1e1127]: Rempel, Kathryn
              - generic [ref=f1e1129]: 619-442-8656
              - generic [ref=f1e1131]: 08-19-2026
              - generic [ref=f1e1133]: SelfPay
              - checkbox [ref=f1e1138] [cursor=pointer]
              - checkbox [checked] [ref=f1e1144] [cursor=pointer]
              - checkbox [checked] [ref=f1e1150] [cursor=pointer]
              - checkbox [ref=f1e1156] [cursor=pointer]
              - checkbox [ref=f1e1162] [cursor=pointer]
              - generic [ref=f1e1168] [cursor=pointer]
            - generic [ref=f1e1171]:
              - checkbox [ref=f1e1174] [cursor=pointer]
              - generic [ref=f1e1177]: Christiansen, Taylor
              - generic [ref=f1e1179]: 991-158-7160
              - generic [ref=f1e1181]: 08-19-2026
              - generic [ref=f1e1183]: SelfPay
              - checkbox [ref=f1e1188] [cursor=pointer]
              - checkbox [checked] [ref=f1e1194] [cursor=pointer]
              - checkbox [checked] [ref=f1e1200] [cursor=pointer]
              - checkbox [ref=f1e1206] [cursor=pointer]
              - checkbox [ref=f1e1212] [cursor=pointer]
              - generic [ref=f1e1218] [cursor=pointer]
            - generic [ref=f1e1221]:
              - checkbox [ref=f1e1224] [cursor=pointer]
              - generic [ref=f1e1227]: VonRueden, Cleo
              - generic [ref=f1e1229]: 938-429-2666
              - generic [ref=f1e1231]: 08-19-2026
              - generic [ref=f1e1233]: SelfPay
              - checkbox [ref=f1e1238] [cursor=pointer]
              - checkbox [checked] [ref=f1e1244] [cursor=pointer]
              - checkbox [checked] [ref=f1e1250] [cursor=pointer]
              - checkbox [ref=f1e1256] [cursor=pointer]
              - checkbox [ref=f1e1262] [cursor=pointer]
              - generic [ref=f1e1268] [cursor=pointer]
            - generic [ref=f1e1271]:
              - checkbox [ref=f1e1274] [cursor=pointer]
              - generic [ref=f1e1277]: Stokes, Mafalda
              - generic [ref=f1e1279]: 679-176-3556
              - generic [ref=f1e1281]: 08-19-2026
              - generic [ref=f1e1283]: SelfPay
              - checkbox [ref=f1e1288] [cursor=pointer]
              - checkbox [checked] [ref=f1e1294] [cursor=pointer]
              - checkbox [checked] [ref=f1e1300] [cursor=pointer]
              - checkbox [ref=f1e1306] [cursor=pointer]
              - checkbox [ref=f1e1312] [cursor=pointer]
              - generic [ref=f1e1318] [cursor=pointer]
            - generic [ref=f1e1321]:
              - checkbox [ref=f1e1324] [cursor=pointer]
              - generic [ref=f1e1327]: Haag, Jeffery
              - generic [ref=f1e1329]: 912-626-9585
              - generic [ref=f1e1331]: 08-19-2026
              - generic [ref=f1e1333]: SelfPay
              - checkbox [ref=f1e1338] [cursor=pointer]
              - checkbox [checked] [ref=f1e1344] [cursor=pointer]
              - checkbox [checked] [ref=f1e1350] [cursor=pointer]
              - checkbox [ref=f1e1356] [cursor=pointer]
              - checkbox [ref=f1e1362] [cursor=pointer]
              - generic [ref=f1e1368] [cursor=pointer]
            - generic [ref=f1e1371]:
              - checkbox [ref=f1e1374] [cursor=pointer]
              - generic [ref=f1e1377]: Wuckert, Wilbert
              - generic [ref=f1e1379]: 699-182-9866
              - generic [ref=f1e1381]: 08-18-2026
              - generic [ref=f1e1383]: SelfPay
              - checkbox [ref=f1e1388] [cursor=pointer]
              - checkbox [checked] [ref=f1e1394] [cursor=pointer]
              - checkbox [checked] [ref=f1e1400] [cursor=pointer]
              - checkbox [ref=f1e1406] [cursor=pointer]
              - checkbox [ref=f1e1412] [cursor=pointer]
              - generic [ref=f1e1418] [cursor=pointer]
            - generic [ref=f1e1421]:
              - checkbox [ref=f1e1424] [cursor=pointer]
              - generic [ref=f1e1427]: Bailey, Travis
              - generic [ref=f1e1429]: 864-536-8485
              - generic [ref=f1e1431]: 08-17-2026
              - generic [ref=f1e1433]: SelfPay
              - checkbox [ref=f1e1438] [cursor=pointer]
              - checkbox [checked] [ref=f1e1444] [cursor=pointer]
              - checkbox [checked] [ref=f1e1450] [cursor=pointer]
              - checkbox [checked] [ref=f1e1456] [cursor=pointer]
              - checkbox [ref=f1e1462] [cursor=pointer]
              - generic [ref=f1e1468] [cursor=pointer]
            - generic [ref=f1e1471]:
              - checkbox [ref=f1e1474] [cursor=pointer]
              - generic [ref=f1e1477]: Goyette, Kayleigh
              - generic [ref=f1e1479]: 716-647-3143
              - generic [ref=f1e1481]: 08-17-2026
              - generic [ref=f1e1483]: SelfPay
              - checkbox [ref=f1e1488] [cursor=pointer]
              - checkbox [checked] [ref=f1e1494] [cursor=pointer]
              - checkbox [checked] [ref=f1e1500] [cursor=pointer]
              - checkbox [ref=f1e1506] [cursor=pointer]
              - checkbox [ref=f1e1512] [cursor=pointer]
              - generic [ref=f1e1518] [cursor=pointer]
            - generic [ref=f1e1521]:
              - checkbox [ref=f1e1524] [cursor=pointer]
              - generic [ref=f1e1527]: Cremin, Wade
              - generic [ref=f1e1529]: 799-467-8681
              - generic [ref=f1e1531]: 08-17-2026
              - generic [ref=f1e1533]: SelfPay
              - checkbox [ref=f1e1538] [cursor=pointer]
              - checkbox [checked] [ref=f1e1544] [cursor=pointer]
              - checkbox [checked] [ref=f1e1550] [cursor=pointer]
              - checkbox [ref=f1e1556] [cursor=pointer]
              - checkbox [ref=f1e1562] [cursor=pointer]
              - generic [ref=f1e1568] [cursor=pointer]
            - generic [ref=f1e1571]:
              - checkbox [ref=f1e1574] [cursor=pointer]
              - generic [ref=f1e1577]: Walsh, Aubrey
              - generic [ref=f1e1579]: 912-040-3864
              - generic [ref=f1e1581]: 08-10-2026
              - generic [ref=f1e1583]: SelfPay
              - checkbox [ref=f1e1588] [cursor=pointer]
              - checkbox [checked] [ref=f1e1594] [cursor=pointer]
              - checkbox [checked] [ref=f1e1600] [cursor=pointer]
              - checkbox [ref=f1e1606] [cursor=pointer]
              - checkbox [ref=f1e1612] [cursor=pointer]
              - generic [ref=f1e1618] [cursor=pointer]
            - generic [ref=f1e1621]:
              - checkbox [ref=f1e1624] [cursor=pointer]
              - generic [ref=f1e1627]: Maggio, Theodore
              - generic [ref=f1e1629]: 860-397-1215
              - generic [ref=f1e1631]: 08-10-2026
              - generic [ref=f1e1633]: SelfPay
              - checkbox [ref=f1e1638] [cursor=pointer]
              - checkbox [checked] [ref=f1e1644] [cursor=pointer]
              - checkbox [checked] [ref=f1e1650] [cursor=pointer]
              - checkbox [ref=f1e1656] [cursor=pointer]
              - checkbox [ref=f1e1662] [cursor=pointer]
              - generic [ref=f1e1668] [cursor=pointer]
            - generic [ref=f1e1671]:
              - progressbar [ref=f1e1672]
              - generic [ref=f1e1675]: Loading more...
  - generic [ref=f1e1682]:
    - generic [ref=f1e1683]:
      - heading "NEW ENROLLMENT" [level=6] [ref=f1e1686]
      - generic [ref=f1e1687]:
        - button [ref=f1e1688] [cursor=pointer]:
          - heading "Cancel" [level=6] [ref=f1e1689]
        - button [ref=f1e1690] [cursor=pointer]:
          - heading "Add Plan" [level=6] [ref=f1e1691]
    - generic [ref=f1e1693]:
      - generic [ref=f1e1694]:
        - heading [level=3] [ref=f1e1695]:
          - button "1 New Enrollment" [expanded] [ref=f1e1696] [cursor=pointer]:
            - generic [ref=f1e1698]:
              - generic [ref=f1e1699]: "1"
              - generic [ref=f1e1700]: New Enrollment
        - region [ref=f1e1707]:
          - generic [ref=f1e1710]:
            - generic [ref=f1e1712]:
              - generic [ref=f1e1713]: Select Patient*
              - generic [ref=f1e1717]:
                - combobox "Search" [ref=f1e1718]: Schuppe, Ronnie
                - button "Open" [ref=f1e1720] [cursor=pointer]
                - group
            - generic [ref=f1e1723]:
              - generic [ref=f1e1724]: Date Of Birth*
              - generic [ref=f1e1727]:
                - button "Choose date, selected date is Mar 27, 2023" [ref=f1e1729] [cursor=pointer]
                - textbox "MM-DD-YYYY" [ref=f1e1732]: 03-27-2023
                - group
            - generic [ref=f1e1733]:
              - generic [ref=f1e1734]: Phone Number*
              - generic [ref=f1e1736]:
                - generic [ref=f1e1739]:
                  - combobox [ref=f1e1740]: "+1"
                  - group
                - textbox "Enter Number" [ref=f1e1742]: 649-665-5874
            - generic [ref=f1e1743]:
              - generic [ref=f1e1744]: Email Address
              - textbox "Enter Email" [ref=f1e1746]
            - generic [ref=f1e1747]:
              - generic [ref=f1e1748]:
                - generic [ref=f1e1749]: Insurance
                - button "Add New Insurance" [ref=f1e1750] [cursor=pointer]
              - generic [ref=f1e1757]:
                - combobox "Search & Select Insurance" [ref=f1e1758]
                - button "Open" [ref=f1e1760] [cursor=pointer]
                - group
            - generic [ref=f1e1763]:
              - generic [ref=f1e1764]: Service*
              - generic [ref=f1e1766]:
                - combobox "Remote Therapeutic Monitoring (RTM)" [ref=f1e1767] [cursor=pointer]
                - textbox: RTM
                - group
            - generic [ref=f1e1769]:
              - generic [ref=f1e1770]: Provider*
              - generic [ref=f1e1774]:
                - combobox "Search & Select Provider" [ref=f1e1775]
                - button "Open" [ref=f1e1777] [cursor=pointer]
                - group
            - generic [ref=f1e1780]:
              - generic [ref=f1e1781]: Condition*
              - generic [ref=f1e1784]:
                - combobox "Search & Select Diagnoses" [ref=f1e1785]
                - button "Open" [ref=f1e1787] [cursor=pointer]
                - group
            - generic [ref=f1e1792]:
              - generic [ref=f1e1793]: Primary Care Manager*
              - generic [ref=f1e1797]:
                - combobox "Search & Select Primary Care Manager" [ref=f1e1798]
                - button "Open" [ref=f1e1800] [cursor=pointer]
                - group
            - generic [ref=f1e1803]:
              - generic [ref=f1e1804]: Secondary Care Manager
              - generic [ref=f1e1806]:
                - combobox "Search & Select Secondary Care Manager" [ref=f1e1807]
                - button "Open" [ref=f1e1809] [cursor=pointer]
                - group
            - generic [ref=f1e1813]:
              - generic [ref=f1e1814]: Location*
              - generic [ref=f1e1818]:
                - combobox "Search & Select Location" [ref=f1e1819]
                - button "Open" [ref=f1e1821] [cursor=pointer]
                - group
            - generic [ref=f1e1824]:
              - generic [ref=f1e1825] [cursor=pointer]:
                - checkbox "Send Consent" [ref=f1e1827]
                - generic [ref=f1e1830]: Send Consent
              - paragraph [ref=f1e1831]: Consent is sent automatically. Only use this if automated consent is offline.
      - heading [level=3] [ref=f1e1833]:
        - button "2 Create Plan" [ref=f1e1834] [cursor=pointer]:
          - generic [ref=f1e1836]:
            - generic [ref=f1e1837]: "2"
            - generic [ref=f1e1838]: Create Plan
      - heading [level=3] [ref=f1e1843]:
        - button "3 Manage Devices" [ref=f1e1844] [cursor=pointer]:
          - generic [ref=f1e1846]:
            - generic [ref=f1e1847]: "3"
            - generic [ref=f1e1848]: Manage Devices
```

# Test source

```ts
  1   | import { test, expect } from '@playwright/test';
  2   | import { ProviderLoginPage } from '../../../../pages/web/provider-portal/login.page';
  3   | import { ProviderEnrollmentsPage } from '../../../../pages/web/provider-portal/enrollment/enrollments.page';
  4   | import { PatientManagementPage } from '../../../../pages/web/provider-portal/care-team-worklist/patient-management.page';
  5   | import { PatientChartPage } from '../../../../pages/web/provider-portal/patient-wallet/patient-chart.page';
  6   | import { PatientDataFactory } from '../../../../utils/PatientDataFactory';
  7   | import { getEnvironmentConfig } from '../../../../config/environment.config';
  8   | import { Logger } from '../../../../utils/logger';
  9   | 
  10  | /**
  11  |  * Verify threshold values (Min/Max) configuration for vitals trigger
  12  |  * alerts on out-of-range readings.
  13  |  *
  14  |  *   Phase 0  Create a brand-new patient.
  15  |  *   Phase 1  In the New Enrollment form, fill Section 1 (Service =
  16  |  *            RPM, Provider, Condition, Primary Care Manager).
  17  |  *   Phase 2  In Section 2 "Create Plan", Heart Rate is auto-added as
  18  |  *            an RPM default vital — locate its config block and
  19  |  *            overwrite Min/Max to known values (MIN/MAX). Verify the
  20  |  *            values are reflected in the inputs.
  21  |  *   Phase 3  Submit the enrollment.
  22  |  *   Phase 4  Activate the patient via Care Team Work List → RPM → NEW
  23  |  *            → click patient → Activate. Newly enrolled patients sit
  24  |  *            in "New" status until activated; vital readings on an
  25  |  *            inactive enrollment do not generate alerts.
  26  |  *   Phase 5  Open the patient chart, RPM → Vitals, add a Heart Rate
  27  |  *            reading at currentMin - 1. Verify an alert is generated for
  28  |  *            the patient on the global Alerts page.
  29  |  *   Phase 6  Add a Heart Rate reading at currentMax + 1 and verify a second
  30  |  *            alert appears.
  31  |  */
  32  | test.describe('Care Plan vital threshold triggers alert on out-of-range readings', () => {
  33  |     test.describe.configure({ mode: 'serial' });
  34  | 
  35  |     const env = getEnvironmentConfig();
  36  |     // Single-vital test: remove all default RPM vital chips except
  37  |     // Blood Glucose so the assertion is unambiguous about which vital
  38  |     // generated the alert. Per the scenario, the thresholds are the
  39  |     // product's configured Min/Max — we VERIFY (not set) them, then
  40  |     // use them as the boundary for the alert test.
  41  |     const VITAL_NAME = 'Blood Glucose';
  42  |     const KEEP_CHIPS = new Set([VITAL_NAME]);
  43  | 
  44  |     test('Reading below Min and above Max each generate an alert for the patient', async ({ page }) => {
  45  |         test.setTimeout(420000);
  46  | 
  47  |         const login = new ProviderLoginPage(page);
  48  |         const patientMgmt = new PatientManagementPage(page);
  49  |         const enrollment = new ProviderEnrollmentsPage(page);
  50  |         const chart = new PatientChartPage(page);
  51  | 
  52  |         Logger.step('=== Care Plan threshold triggers alert (Min/Max) ===');
  53  | 
  54  |         // ── PHASE 0: Login + create a new patient ────────────────────────
  55  |         Logger.step('Phase 0: Login as provider and create a new patient');
  56  |         await page.goto(env.providerPortalUrl);
  57  |         await login.login(env.providerCredentials.username, env.providerCredentials.password);
  58  | 
  59  |         const patient = PatientDataFactory.createPatient();
  60  |         const patientFullName = `${patient.lastName}, ${patient.firstName}`;
  61  |         const patientLastName = patient.lastName;
  62  |         Logger.info(`New patient: ${patientFullName}`);
  63  |         await patientMgmt.patientCreation(patient.firstName, patient.lastName, patient.dob, patient.phoneNumber);
  64  | 
  65  |         // After patientCreation, the app may show a confirmation dialog:
  66  |         // "DO YOU WANT TO ENROLL THIS PATIENT INTO A PROGRAM?" with a
  67  |         // "+" / "Yes" affordance. Click it to open the New Enrollment
  68  |         // form. Skip if not present (older flow opens the form directly).
  69  |         const enrollPromptVisible = await page
  70  |             .getByText(/DO YOU WANT TO ENROLL THIS PATIENT/i)
  71  |             .isVisible({ timeout: 5000 })
  72  |             .catch(() => false);
  73  |         if (enrollPromptVisible) {
  74  |             const enrollConfirm = page
  75  |                 .getByRole('button', { name: /^(Yes|Enroll|Add)$/i })
  76  |                 .or(page.locator("//div[contains(.,'DO YOU WANT TO ENROLL')]//button"))
  77  |                 .first();
  78  |             await enrollConfirm.waitFor({ state: 'visible', timeout: 5000 });
  79  |             await enrollConfirm.click();
  80  |             Logger.info('Dismissed "Enroll patient into program?" confirmation');
  81  |         }
  82  | 
  83  |         // Now wait for the NEW ENROLLMENT form heading.
> 84  |         await page.locator('//h5[text()="NEW ENROLLMENT"]').waitFor({ state: 'visible', timeout: 15000 });
      |                                                             ^ TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
  85  |         Logger.info('Phase 0 ✓ Patient created; enrollment form is open');
  86  | 
  87  |         // ── PHASE 1: Fill Section 1 (Service = RPM, Provider, CM, etc.) ──
  88  |         Logger.step('Phase 1: Fill enrollment Section 1 with Service = RPM');
  89  |         const rpmService = 'Remote Patient Monitoring (RPM)';
  90  | 
  91  |         await enrollment.serviceDropdown.click();
  92  |         await page.locator(`//li[text()="${rpmService}"]`).first().click();
  93  |         await page.waitForTimeout(800);
  94  | 
  95  |         await enrollment.providerDropdown.click();
  96  |         const providerOptions = page.locator('//ul[@role="listbox"]//li');
  97  |         await providerOptions.first().waitFor({ state: 'visible', timeout: 5000 });
  98  |         await providerOptions.first().click();
  99  |         await page.waitForTimeout(500);
  100 | 
  101 |         await enrollment.careMangerDropdown.click();
  102 |         const cmOptions = page.locator('//ul[@role="listbox"]//li');
  103 |         await cmOptions.first().waitFor({ state: 'visible', timeout: 5000 });
  104 |         await cmOptions.first().click();
  105 |         await page.waitForTimeout(500);
  106 | 
  107 |         await enrollment.conditionsDropdown.click();
  108 |         await page.locator("//li[@id='tags-standard-option-0']//input").first().click();
  109 |         await page.locator("//li[@id='tags-standard-option-2']//input").first().click();
  110 |         await page.keyboard.press('Escape');
  111 |         await page.waitForTimeout(500);
  112 |         Logger.info('Phase 1 ✓ Section 1 filled');
  113 | 
  114 |         // ── PHASE 2: Keep only Blood Glucose + configure its Min/Max ─────
  115 |         Logger.step(`Phase 2: Keep only ${VITAL_NAME} chip, then read and verify its Min/Max thresholds`);
  116 | 
  117 |         // The enrollment form modal scrolls independently. Scroll to
  118 |         // its bottom so Section 2's body (Vitals chips + config blocks)
  119 |         // renders into the viewport. If Section 2 happens to be
  120 |         // collapsed afterwards, click its toggle to expand.
  121 |         const vitalsLabel = page.locator("//*[contains(normalize-space(),'Vitals')]").first();
  122 |         // First: scroll the modal to the bottom.
  123 |         await page.evaluate(() => {
  124 |             const dialog = document.querySelector('[role="dialog"], .MuiDialog-paper, .MuiDrawer-paper');
  125 |             if (dialog) dialog.scrollTop = dialog.scrollHeight;
  126 |             else window.scrollTo(0, document.body.scrollHeight);
  127 |         });
  128 |         await page.waitForTimeout(500);
  129 | 
  130 |         // If Vitals isn't visible yet, click the Create Plan toggle.
  131 |         let vitalsVisible = await vitalsLabel.isVisible({ timeout: 2000 }).catch(() => false);
  132 |         if (!vitalsVisible) {
  133 |             const createPlanToggle = page
  134 |                 .getByRole('button', { name: /^\s*2\s*Create Plan\s*$/i })
  135 |                 .first();
  136 |             await createPlanToggle.scrollIntoViewIfNeeded();
  137 |             await createPlanToggle.click();
  138 |             await page.waitForTimeout(800);
  139 |             vitalsVisible = await vitalsLabel.isVisible({ timeout: 5000 }).catch(() => false);
  140 |         }
  141 |         expect(vitalsVisible, 'Section 2 "Create Plan" body (Vitals row) must be visible').toBe(true);
  142 |         Logger.info('Section 2 "Create Plan" body is visible');
  143 |         await page.waitForTimeout(500);
  144 | 
  145 |         // Remove every default vital chip except VITAL_NAME so only
  146 |         // its config block remains. Chips render as MUI Autocomplete
  147 |         // tags with an X icon; each tag's accessible label / text is
  148 |         // the vital name (e.g., "Blood Pressure", "Body Mass Index").
  149 |         Logger.step(`Removing all vital chips except "${VITAL_NAME}"`);
  150 |         // Each removal removes a chip — the list re-renders, so loop
  151 |         // until only the keep-set chips remain (cap iterations to
  152 |         // avoid runaway loops on UI bugs).
  153 |         for (let iter = 0; iter < 12; iter++) {
  154 |             const chips = page.locator(
  155 |                 "//div[contains(@class,'MuiAutocomplete-tag') or contains(@class,'MuiChip-root')]",
  156 |             );
  157 |             const chipCount = await chips.count();
  158 |             let removedAny = false;
  159 |             for (let i = 0; i < chipCount; i++) {
  160 |                 const chipText = ((await chips.nth(i).textContent()) || '').trim();
  161 |                 if (KEEP_CHIPS.has(chipText)) continue;
  162 |                 // Click the chip's X (close) button to remove it.
  163 |                 const closeBtn = chips
  164 |                     .nth(i)
  165 |                     .locator("svg[data-testid='CancelIcon'], [aria-label*='delete' i], button");
  166 |                 if ((await closeBtn.count()) === 0) continue;
  167 |                 await closeBtn.first().click({ force: true });
  168 |                 await page.waitForTimeout(300);
  169 |                 removedAny = true;
  170 |                 break; // re-evaluate chips after each removal
  171 |             }
  172 |             if (!removedAny) break;
  173 |         }
  174 |         const remainingChips = page.locator(
  175 |             "//div[contains(@class,'MuiAutocomplete-tag') or contains(@class,'MuiChip-root')]",
  176 |         );
  177 |         const remainingTexts = (await remainingChips.allTextContents()).map((t) => t.trim()).filter(Boolean);
  178 |         Logger.info(`Remaining chips after pruning: ${JSON.stringify(remainingTexts)}`);
  179 |         expect(
  180 |             remainingTexts,
  181 |             `Only "${VITAL_NAME}" should remain in the Vitals chip list (saw ${JSON.stringify(remainingTexts)})`,
  182 |         ).toEqual([VITAL_NAME]);
  183 | 
  184 |         // With only Blood Glucose remaining, its config block is the
```