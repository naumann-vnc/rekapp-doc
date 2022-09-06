ssh2env 1000042046 48


OTC.cosid:
1000035665

sudo systemctl status check_mk.socket
sudo systemctl restart check_mk.socket

sudo systemctl status sshd
sudo systemctl status wildfly

Server went down due to the nightly restart of the Wildfly server. Brought it back manually, the issue is now resolved.
Alert generated due to the nightly restart of the Wildfly server. Brought it back manually, the issue is now resolved.

False positive alert from Check_MK, does not represent an issue to the customer.

Alert generated due to the nightly restart of the Wildfly server. The issue was resolved as the service automatically started.

Alert generated due to a scheduled Windows update.
Server went down due to a scheduled Windows update.

Alert generated due to a misconfigured Crontab that rebooted the Wildfly server, the server was brought back manually and the configuratin was fixed.