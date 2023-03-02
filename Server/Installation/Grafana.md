```shell
docker exect -it --user root "$(docker ps -l -q --filter="NAME=grafana")" bash "sed -i -e ''"

vi /usr/share/grafana/conf/defaults.ini

[auth.anonymous]
enabled = false

org_name = Rekapp

hide version = true

```