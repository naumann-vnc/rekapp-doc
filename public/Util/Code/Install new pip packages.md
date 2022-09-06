
```shell
export http_proxy="i1000007:8080"
export https_proxy="i1000007:8080"
```

```shell
python -m pip install $package_name
```

```shell
sudo bash -c 'for sp in /usr/local/lib /usr/local/lib64; do cd $sp; for d in $(find . -name "*" -type d); do chmod 755 $d; done; for f in $(find . -name "*" -type f); do chmod 644 $f; done; done'
```
