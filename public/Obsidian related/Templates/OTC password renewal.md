This is a template for the **Implementation procedure** portion of a Let's Encrypt certificate renewall change request, follow these next steps to properly use the template:
1. Remove all uncessary environments(ones that won't be updated)

---
# ITE MGT
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000099999 -t OTC00000000001000001672
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000099999 -t OTC00000000001000001672
 
prv mgt credential crd.mgt.json #
 
/opt/prv/public/tools/changeotcpassword_2.sh -h 1000099999 -t OTC00000000001000001672
 
prv mgt vm_acc --createTest #
```
---
# 8400000100
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8400000100 -t OTC-EU-DE-00000000001000041921
/opt/prv/public/tools/changeotcpassword_1.sh -h 8400000100 -t OTC-EU-DE-00000000001000041921
  
prv 8400000100 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8400000100 -t OTC-EU-DE-00000000001000041921
 
prv 8400000100 vm_crd --patchcrdcontent #
prv 8400000100 vm_acc --createTest #
```
---
# 8400000200
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8400000200 -t OTC-EU-DE-00000000001000041922
/opt/prv/public/tools/changeotcpassword_1.sh -h 8400000200 -t OTC-EU-DE-00000000001000041922
  
prv 8400000200 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8400000200 -t OTC-EU-DE-00000000001000041922
 
prv 8400000200 vm_crd --patchcrdcontent #
prv 8400000200 vm_acc --createTest #
```
---
# 8400000300
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8400000300 -t OTC-EU-DE-00000000001000041923
/opt/prv/public/tools/changeotcpassword_1.sh -h 8400000300 -t OTC-EU-DE-00000000001000041923
  
prv 8400000300 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8400000300 -t OTC-EU-DE-00000000001000041923
 
prv 8400000300 vm_crd --patchcrdcontent #
prv 8400000300 vm_acc --createTest #
```
---
# 8400000400
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8400000400 -t OTC-EU-DE-00000000001000041924
/opt/prv/public/tools/changeotcpassword_1.sh -h 8400000400 -t OTC-EU-DE-00000000001000041924
  
prv 8400000400 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8400000400 -t OTC-EU-DE-00000000001000041924
 
prv 8400000400 vm_crd --patchcrdcontent #
prv 8400000400 vm_acc --createTest #
```
---
# 8400000500
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8400000500 -t OTC-EU-DE-00000000001000041925
/opt/prv/public/tools/changeotcpassword_1.sh -h 8400000500 -t OTC-EU-DE-00000000001000041925
  
prv 8400000500 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8400000500 -t OTC-EU-DE-00000000001000041925
 
prv 8400000500 vm_crd --patchcrdcontent #
prv 8400000500 vm_acc --createTest #
```
---
# 8400000600
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8400000600 -t OTC00000000001000000725
/opt/prv/public/tools/changeotcpassword_1.sh -h 8400000600 -t OTC00000000001000000725
 
prv 8400000600 credential crd.hst.json #
 
/opt/prv/public/tools/changeotcpassword_2.sh -h 8400000600 -t OTC00000000001000000725
 
prv 8400000600 vm_crd --patchcrdcontent #
prv 8400000600 vm_acc --createTest #
```
---
# PRD

# KAESER
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000033015 -t OTC-EU-DE-00000000001000020792
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000033015 -t OTC-EU-DE-00000000001000020792

prv 1000033015 credential crd.hst.json #

/opt/prv/public/tools/changeotcpassword_2.sh -h 1000033015 -t OTC-EU-DE-00000000001000020792

prv 1000033015 vm_crd --patchcrdcontent  #
prv 1000033015 vm_acc --createTest #
```
---
# CARRIER DEV
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8810000120 -t OTC-EU-DE-00000000001000035663
/opt/prv/public/tools/changeotcpassword_1.sh -h 8810000120 -t OTC-EU-DE-00000000001000035663
 
prv 8810000120 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8810000120 -t OTC-EU-DE-00000000001000035663
 
prv 8810000120 vm_acc --createTest #
```
---
# CARRIER PPR
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8810000140 -t OTC-EU-DE-00000000001000035664
/opt/prv/public/tools/changeotcpassword_1.sh -h 8810000140 -t OTC-EU-DE-00000000001000035664
 
prv 8810000140 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8810000140 -t OTC-EU-DE-00000000001000035664
 
prv 8810000140 vm_acc --createTest #
```
---
# CARRIER PRD
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000042046 -t OTC-EU-DE-00000000001000035665
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000042046 -t OTC-EU-DE-00000000001000035665
 
prv 1000042046 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 1000042046 -t OTC-EU-DE-00000000001000035665
 
prv 1000042046 vm_acc --createTest #

```
---
# MAGNA
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000046216 -t OTC-EU-DE-00000000001000041917
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000046216 -t OTC-EU-DE-00000000001000041917
 
prv 1000046216 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 1000046216 -t OTC-EU-DE-00000000001000041917
 
prv 1000046216 vm_crd --patchcrdcontent  #
prv 1000046216 vm_acc --createTest #
```
---
# Shell
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8800000200 -t OTC-EU-DE-00000000001000041918
/opt/prv/public/tools/changeotcpassword_1.sh -h 8800000200 -t OTC-EU-DE-00000000001000041918
 
prv 8800000200 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8800000200 -t OTC-EU-DE-00000000001000041918
 
prv 8800000200 vm_crd --patchcrdcontent  #
prv 8800000200 vm_acc --createTest #
```
---
# Recaro
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000088874 -t OTC-EU-DE-00000000001000041920
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000088874 -t OTC-EU-DE-00000000001000041920
 
prv 1000088874 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 1000088874 -t OTC-EU-DE-00000000001000041920
 
prv 1000088874 vm_crd --patchcrdcontent  #
prv 1000088874 vm_acc --createTest #
```
---
# EDAG
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000027361 -t OTC-EU-DE-00000000001000020790
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000027361 -t OTC-EU-DE-00000000001000020790
 
prv 1000027361 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 1000027361 -t OTC-EU-DE-00000000001000020790
 
prv 1000027361 vm_crd --patchcrdcontent #
prv 1000027361 vm_acc --createTest #
```
---
# MUM
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000035729 -t OTC-EU-DE-00000000001000035661
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000035729 -t OTC-EU-DE-00000000001000035661
 
prv 1000035729 credential crd.hst.json #
 
/opt/prv/public/tools/changeotcpassword_2.sh -h 1000035729 -t OTC-EU-DE-00000000001000035661
 
prv 1000035729 vm_crd --patchcrdcontent #
prv 1000035729 vm_acc --createTest #
```
---
# TECOSIM
```shell
/opt/prv/public/tools/testuserlogin.sh -h 1000050198 -t OTC-EU-DE-00000000001000035662
/opt/prv/public/tools/changeotcpassword_1.sh -h 1000050198 -t OTC-EU-DE-00000000001000035662
 
prv 1000050198 credential crd.hst.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 1000050198 -t OTC-EU-DE-00000000001000035662
 
prv 1000050198 vm_crd --patchcrdcontent #
prv 1000050198 vm_acc --createTest #
```
---
# MGT
```shell
/opt/prv/public/tools/testuserlogin.sh -h 8800000000 -t OTC-EU-DE-00000000001000020789
/opt/prv/public/tools/changeotcpassword_1.sh -h 8800000000 -t OTC-EU-DE-00000000001000020789
 
prv 8800000000 credential crd.mgt.json #
  
/opt/prv/public/tools/changeotcpassword_2.sh -h 8800000000 -t OTC-EU-DE-00000000001000020789
 
prv 8800000000 vm_acc --createTest #
```