```shell
docker pull dpage/pgadmin4:latest

docker run -p 5050:5050 \
    -e "PGADMIN_DEFAULT_EMAIL=admin@rekapp.net" \
    -e "PGADMIN_DEFAULT_PASSWORD=admin" \
    -d dpage/pgadmin4
```