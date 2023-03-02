https://techviewleo.com/install-postgresql-12-on-amazon-linux/
```shell
sudo yum install postgresql12 postgresql12-server

/usr/pgsql-12/bin/postgresql-12-setup initdb
#sudo systemctl start postgresql-12
sudo systemctl enable postgresql-12
sudo systemctl status postgresql-12

sudo -u postgres psql
```
DB installation:
```shell
sudo -u postgres psql
create database dbpython;
```

```shell
postgres=# \l
 dbpython  | postgres | UTF8     | en_US.UTF-8 | en_US.UTF-8 |
 postgres  | postgres | UTF8     | en_US.UTF-8 | en_US.UTF-8 |
 template0 | postgres | UTF8     | en_US.UTF-8 | en_US.UTF-8 | =c/postgres          +
           |          |          |             |             | postgres=CTc/postgres
 template1 | postgres | UTF8     | en_US.UTF-8 | en_US.UTF-8 | =c/postgres          +
           |          |          |             |             | postgres=CTc/postgres
```

```shell
\c dbpython
```

---

/var/lib/pgsql/12/data/pg_hba.conf
```shell
# TYPE  DATABASE        USER            ADDRESS                 METHOD
#local    postgres     postgres     peer
# "local" is for Unix domain socket connections only
local   all             all                                     md5
# IPv4 local connections:
host    all             all             127.0.0.1/32            md5
# IPv6 local connections:
host    all             all             ::1/128                 md5
# Allow replication connections from localhost, by a user with the
# replication privilege.
local   replication     all                                     md5
host    replication     all             127.0.0.1/32            md5
host    replication     all             ::1/128                 md5
```
