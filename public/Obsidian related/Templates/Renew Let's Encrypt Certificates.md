This is a template for the **Implementation procedure** portion of a Let's Encrypt certificate renewall change request, follow these next steps to properly use the template:
1. Remove all uncessary environments(ones that won't be updated)
2. Use the "Replace" tool on the top right "More options" menu to find "$date" and replace it with the day's timestamp, eg. 20220907
3. Replace the certificate information with the current certificateexpiration.txt file found in mgt.prv:/opt/prv/public/credentials

---

# Implementation procedure

## ITE
8400000101 crd.gst.json 2022-07-19 2022-10-17 hpc_plmcloud_tsystemsservice_com_cer  
8400000101 crd.gst.json 2022-07-19 2022-10-17 wad_plmcloud_tsystemsservice_com_cer  
8400000101 crd.gst.json 2022-07-19 2022-10-17 wpl_plmcloud_tsystemsservice_com_cer

```shell
# turn on servers on OTC tenant OTC-EU-DE-00000000001000041921
cp -pr /opt/prv/public/credentials/8400000101 /opt/prv/public/credentials/archive/8400000101_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 8400000100 8400000101 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 8400000100 8400000101 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 8400000100 8400000101 crd.gst.json

prv 8400000100 8400000101 vm_acc --patchstdcertificates #
```
---
8400000201 crd.gst.json 2022-07-19 2022-10-17 hpc_plmcloud_tsystemsservice_com_cer  
8400000201 crd.gst.json 2022-07-19 2022-10-17 wad_plmcloud_tsystemsservice_com_cer  
8400000201 crd.gst.json 2022-07-19 2022-10-17 wpl_plmcloud_tsystemsservice_com_cer

```shell
# turn on servers on OTC tenant OTC-EU-DE-00000000001000041922
cp -pr /opt/prv/public/credentials/8400000201 /opt/prv/public/credentials/archive/8400000201_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 8400000200 8400000201 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 8400000200 8400000201 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 8400000200 8400000201 crd.gst.json

prv 8400000200 8400000201 vm_acc --patchstdcertificates #
```
---
8400000301 crd.gst.json 2022-07-19 2022-10-17 hpc_plmcloud_tsystemsservice_com_cer  
8400000301 crd.gst.json 2022-07-19 2022-10-17 wad_plmcloud_tsystemsservice_com_cer  
8400000301 crd.gst.json 2022-07-19 2022-10-17 wpl_plmcloud_tsystemsservice_com_cer

```shell
# turn on servers on OTC tenant OTC-EU-DE-00000000001000041923
cp -pr /opt/prv/public/credentials/8400000301 /opt/prv/public/credentials/archive/8400000301_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 8400000300 8400000301 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 8400000300 8400000301 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 8400000300 8400000301 crd.gst.json

prv 8400000300 8400000301 vm_acc --patchstdcertificates #
```
---
8400000401 crd.gst.json 2022-07-19 2022-10-17 hpc_plmcloud_tsystemsservice_com_cer  
8400000401 crd.gst.json 2022-07-19 2022-10-17 wad_plmcloud_tsystemsservice_com_cer  
8400000401 crd.gst.json 2022-07-19 2022-10-17 wpl_plmcloud_tsystemsservice_com_cer

```shell
# turn on servers on OTC tenant OTC-EU-DE-00000000001000041924
cp -pr /opt/prv/public/credentials/8400000401 /opt/prv/public/credentials/archive/8400000401_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 8400000400 8400000401 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 8400000400 8400000401 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 8400000400 8400000401 crd.gst.json

prv 8400000400 8400000401 vm_acc --patchstdcertificates #
```
---
8400000501 crd.gst.json 2022-07-19 2022-10-17 hpc_plmcloud_tsystemsservice_com_cer  
8400000501 crd.gst.json 2022-07-19 2022-10-17 wad_plmcloud_tsystemsservice_com_cer  
8400000501 crd.gst.json 2022-07-19 2022-10-17 wpl_plmcloud_tsystemsservice_com_cer

```shell
# turn on servers on OTC tenant OTC-EU-DE-00000000001000041925
cp -pr /opt/prv/public/credentials/8400000501 /opt/prv/public/credentials/archive/8400000501_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 8400000500 8400000501 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 8400000500 8400000501 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 8400000500 8400000501 crd.gst.json

prv 8400000500 8400000501 vm_acc --patchstdcertificates #
```
---
8400000601 crd.gst.json 07/01/2022 07/04/2022 hpc_plmcloud_tsystemsservice_com_cer
8400000601 crd.gst.json 07/01/2022 07/04/2022 tcr_plmcloud_tsystemsservice_com_cer  
8400000601 crd.gst.json 07/01/2022 07/04/2022 wad_plmcloud_tsystemsservice_com_cer  
8400000601 crd.gst.json 07/01/2022 07/04/2022 wpl_plmcloud_tsystemsservice_com_cer

```shell
# turn on servers on OTC tenant OTC00000000001000000725
cp -pr /opt/prv/public/credentials/8400000601 /opt/prv/public/credentials/archive/8400000601_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 8400000600 8400000601 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh tcr_plmcloud_tsystemsservice_com 8400000600 8400000601 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 8400000600 8400000601 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 8400000600 8400000601 crd.gst.json
prv 8400000600 8400000601 vm_acc --patchstdcertificates #
```
---
1000099999 crd.mgt.json 2022-06-24 2022-09-22 acc_plmcloud_tsystemsservice_com_cer  
1000099999 crd.mgt.json 2022-06-24 2022-09-22 mon_plmcloud_tsystemsservice_com_cer  
1000099999 crd.mgt.json 2022-06-24 2022-09-22 prv_plmcloud_tsystemsservice_com_cer  
1000099999 crd.mgt.json 2022-06-24 2022-09-22 ssp_plmcloud_tsystemsservice_com_cer

```shell
#turn on servers on OTC tenant OTC00000000001000001672
cp -pr /opt/prv/public/credentials/1000099999 /opt/prv/public/credentials/archive/1000099999_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh acc_plmcloud_tsystemsservice_com 1000099999 1000099999 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh mon_plmcloud_tsystemsservice_com 1000099999 1000099999 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh prv_plmcloud_tsystemsservice_com 1000099999 1000099999 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh ssp_plmcloud_tsystemsservice_com 1000099999 1000099999 crd.mgt.json
prv mgt vm_acc --patchdomaincertificates #
prv mgt vm_prv --patchdomaincertificates #
```

---

# PRD

EDAG  
1000027361 crd.gst.json 2022-06-24 2022-09-22 hpc_plmcloud_tsystemsservice_com_cer  
1000027361 crd.gst.json 2022-06-24 2022-09-22 wad_plmcloud_tsystemsservice_com_cer  
1000027361 crd.gst.json 2022-06-24 2022-09-22 wpl_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/1000027361 /opt/prv/public/credentials/archive/1000027361_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 1000027361 1000027361 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 1000027361 1000027361 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 1000027361 1000027361 crd.gst.json
prv 1000027361 1000027361 vm_acc --patchstdcertificates #
```
---
KAESER
1000033015 crd.gst.json 07/01/2022 07/04/2022 hpc_plmcloud_tsystemsservice_com_cer  
1000033015 crd.gst.json 07/01/2022 07/04/2022 wad_plmcloud_tsystemsservice_com_cer  
1000033015 crd.gst.json 07/01/2022 07/04/2022 wpl_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/1000033015 /opt/prv/public/credentials/archive/1000033015_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh --create hpc_plmcloud_tsystemsservice_com 1000033015 1000033015 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh --create wad_plmcloud_tsystemsservice_com 1000033015 1000033015 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh --create wpl_plmcloud_tsystemsservice_com 1000033015 1000033015 crd.gst.json
prv 1000033015 1000033015 vm_acc --patchstdcertificates #
```
---
MAGNA

1000046216 crd.gst.json 2022-07-04 2022-10-02 hpc_plmcloud_tsystemsservice_com_cer
1000046216 crd.gst.json 2022-07-04 2022-10-02 wad_plmcloud_tsystemsservice_com_cer
1000046216 crd.gst.json 2022-07-04 2022-10-02 wpl_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/1000046216 /opt/prv/public/credentials/archive/1000046216_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 1000046216 1000046216 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 1000046216 1000046216 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 1000046216 1000046216 crd.gst.json
prv 1000046216 1000046216 vm_acc --patchstdcertificates #
```
---
TECOSIM
1000050198 crd.gst.json 2022-07-04 2022-10-02 hpc_plmcloud_tsystemsservice_com_cer
1000050198 crd.gst.json 2022-07-04 2022-10-02 wad_plmcloud_tsystemsservice_com_cer
1000050198 crd.gst.json 2022-07-04 2022-10-02 wpl_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/1000050198 /opt/prv/public/credentials/archive/1000050198_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 1000050198 1000050198 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 1000050198 1000050198 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 1000050198 1000050198 crd.gst.json
prv 1000050198 1000050198 vm_acc --patchstdcertificates #
```
---
SHELL
8800000200 crd.gst.json 2022-07-04 2022-10-02 hpc_plmcloud_tsystemsservice_com_cer
8800000200 crd.gst.json 2022-07-04 2022-10-02 wad_plmcloud_tsystemsservice_com_cer
8800000200 crd.gst.json 2022-07-04 2022-10-02 wpl_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/8800000200 /opt/prv/public/credentials/archive/8800000200_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 8800000200 8800000201 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 8800000200 8800000201 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 8800000200 8800000201 crd.gst.json
prv 8800000200 8800000201 vm_acc --patchstdcertificates #
```
---
RECARO
1000088874 crd.gst.json 2022-07-04 2022-10-02 hpc_plmcloud_tsystemsservice_com_cer
1000088874 crd.gst.json 2022-07-04 2022-10-02 wad_plmcloud_tsystemsservice_com_cer
1000088874 crd.gst.json 2022-07-04 2022-10-02 wpl_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/1000088874 /opt/prv/public/credentials/archive/1000088874_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh hpc_plmcloud_tsystemsservice_com 1000088874 1000088874 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wad_plmcloud_tsystemsservice_com 1000088874 1000088874 crd.gst.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh wpl_plmcloud_tsystemsservice_com 1000088874 1000088874 crd.gst.json
prv 1000088874 1000088874 vm_acc --patchstdcertificates #
```
---
CARRIER DEV
8810000120 crd.gst.json 2022-08-11 2022-11-09 tcr_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/8810000120 /opt/prv/public/credentials/archive/8810000120_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh tcr_plmcloud_tsystemsservice_com 8810000120 8810000120 crd.gst.json
prv 8810000120 8810000120 vm_acc --patchtcrcertificates #
```
---
CARRIER PPR
8810000140 crd.gst.json 2022-08-23 2022-11-21 tcr_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/8810000140 /opt/prv/public/credentials/archive/8810000140_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh tcr_plmcloud_tsystemsservice_com 8810000140 8810000140 crd.gst.json
prv 8810000140 8810000140 vm_acc --patchtcrcertificates #
```
---
CARRIER PRD
1000042046 crd.gst.json 2022-08-26 2022-11-24 tcr_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/1000042046 /opt/prv/public/credentials/archive/1000042046_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh tcr_plmcloud_tsystemsservice_com 1000042046 1000042046 crd.gst.json
prv 1000042046 1000042046 vm_acc --patchtcrcertificates #
```
---
MGT
8800000000 crd.mgt.json 2022-07-04 2022-10-02 acc_plmcloud_tsystemsservice_com_cer
8800000000 crd.mgt.json 2022-07-04 2022-10-02 dns_plmcloud_tsystemsservice_com_cer
8800000000 crd.mgt.json 2022-07-04 2022-10-02 git_plmcloud_tsystemsservice_com_cer
8800000000 crd.mgt.json 2022-07-04 2022-10-02 mon_plmcloud_tsystemsservice_com_cer
8800000000 crd.mgt.json 2022-07-04 2022-10-02 prv_plmcloud_tsystemsservice_com_cer
8800000000 crd.mgt.json 2022-07-04 2022-10-02 ssp_plmcloud_tsystemsservice_com_cer
```shell
cp -pr /opt/prv/public/credentials/8800000000 /opt/prv/public/credentials/archive/8800000000_$date
/opt/prv/public/tools/letsencryptcreateorrenew.sh acc_plmcloud_tsystemsservice_com 8800000000 8800000000 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh dns_plmcloud_tsystemsservice_com 8800000000 8800000000 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh git_plmcloud_tsystemsservice_com 8800000000 8800000000 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh mon_plmcloud_tsystemsservice_com 8800000000 8800000000 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh prv_plmcloud_tsystemsservice_com 8800000000 8800000000 crd.mgt.json
/opt/prv/public/tools/letsencryptcreateorrenew.sh ssp_plmcloud_tsystemsservice_com 8800000000 8800000000 crd.mgt.json
prv mgt vm_acc --patchdomaincertificates #
prv mgt vm_prv --patchdomaincertificates #
```

