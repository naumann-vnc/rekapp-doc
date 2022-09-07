# [[Carrier DEV 8810000120]]

| Page                    | AWC                                                                  | Expected output/action                                             |
| ----------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Active workspace        | https://tcr.8810000120.plmcloud.t-systems-service.com/awc/           | check awc connection, login and 3D view                            |
| FSC/FMS connection test | https://tcr.8810000120.plmcloud.t-systems-service.com:4544/          | HTTP ERROR 400 expected                                            |
| TC URL                  | https://tcr.8810000120.plmcloud.t-systems-service.com/tc/            | Not Found error expected                                           |
| Documentation URL       | https://tcr.8810000120.plmcloud.t-systems-service.com/tdoc/tc/12/PDF | No connection is expected(documentation server must be turned off) |

---
# [[Carrier PPR 8810000140]]

| Page                    | AWC                                                                  | Expected output/action                  |
| ----------------------- | -------------------------------------------------------------------- | --------------------------------------- |
| Active workspace        | https://tcr.8810000140.plmcloud.t-systems-service.com/awc/           | check awc connection, login and 3D view |
| FSC/FMS connection test | https://tcr.8810000140.plmcloud.t-systems-service.com:4544/          | HTTP ERROR 400 expected                 |
| TC URL                  | https://tcr.8810000140.plmcloud.t-systems-service.com/tc/            | Not Found error expected                |
| Documentation URL       | https://tcr.8810000140.plmcloud.t-systems-service.com/tdoc/tc/12/PDF | Expect documentation page               |

---
# [[Carrier PRD 1000042046]]

| Page                    | AWC                                                                  | Expected output/action                  |
| ----------------------- | -------------------------------------------------------------------- | --------------------------------------- |
| Active workspace        | https://tcr.1000042046.plmcloud.t-systems-service.com/awc/           | check awc connection, login and 3D view |
| FSC/FMS connection test | https://tcr.1000042046.plmcloud.t-systems-service.com:4544/          | HTTP ERROR 400 expected                 |
| TC URL                  | https://tcr.1000042046.plmcloud.t-systems-service.com/tc/            | Not Found error expected                |
| Documentation URL       | https://tcr.1000042046.plmcloud.t-systems-service.com/tdoc/tc/12/PDF | Expect documentation page               |
