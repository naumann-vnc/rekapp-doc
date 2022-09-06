For [[ITE]] environments:

```
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/1000099999/crd.mgt.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/1000099999/crd.mgt.json
```

```
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/8400000100/crd.hst.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/8400000100/crd.hst.json
```

```
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/8400000200/crd.hst.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/8400000200/crd.hst.json
```

```
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/8400000300/crd.hst.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/8400000300/crd.hst.json
```

```
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/8400000400/crd.hst.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/8400000400/crd.hst.json
```

```
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/8400000500/crd.hst.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/8400000500/crd.hst.json
```

```
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/8400000600/crd.hst.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/8400000600/crd.hst.json
```

---
```
#template
sudo jq -r ".parameters .apiadmin_otc_password" /opt/prv/public/credentials/"$hstcsoid"/crd.hst.json
sudo jq -r ".parameters .cus_otc_domainid" /opt/prv/public/credentials/"$hstcsoid"/crd."$file_type".json
```