# Update GitLab
```[opsadmin@prd.mgt.011 ~]$ ssh2env mgt 13```

1. Perform GitLab check:
```gitlab-rake gitlab:check```

2. Check latest security release on: 
https://about.gitlab.com/releases/categories/releases/
If there are releases for the Runner, update them aswell.

3. Find the version you want to update with:
```yum search <gitlab-module> --showduplicates```
```e.g. yum search gitlab-ce --showduplicates```

4. Check if the latest release matches the one found with the **yum search**, e.g.

***The lastest release was 14.5.2:**
___

### GitLab Security Release: 14.5.2, 14.4.4, and 14.3.6
(https://about.gitlab.com/releases/2021/12/06/security-release-gitlab-14-5-2-released/)
[Rohit Shambhuni](https://about.gitlab.com/company/team/#rshambhuni) 
Dec 6, 2021
___

<pre>
gitlab-ce-14.5.0-ce.0.el7.x86_64 : GitLab Community Edition (including NGINX, Postgres, Redis)
gitlab-ce-14.5.1-ce.0.el7.x86_64 : GitLab Community Edition (including NGINX, Postgres, Redis)
<strong>gitlab-ce-14.5.2-ce.0.el7.x86_64 : GitLab Community Edition (including NGINX, Postgres, Redis)</strong>
</pre>

5. Install the GitLab version with:
```yum install <gitlab-version>```
```e.g. yum install gitlab-ce-14.4.1-ce.0.el7```

<details>
  <summary>Expected output</summary>
   <pre>
        _______ __  __          __
    / ____(_) /_/ /   ____ _/ /_
   / / __/ / __/ /   / __ `/ __ \
  / /_/ / / /_/ /___/ /_/ / /_/ /
  \____/_/\__/_____/\__,_/_.___/
  
Upgrade complete! If your GitLab server is misbehaving try running
  sudo gitlab-ctl restart
  before anything else.
If you need to roll back to the previous version you can use the database
backup made during the upgrade (scroll up for the filename).
  Verifying  : gitlab-ce-14.5.2-ce.0.el7.x86_64                                                                                                                   1/2
  Verifying  : gitlab-ce-14.4.1-ce.0.el7.x86_64                                                                                                                   2/2
Updated:
  gitlab-ce.x86_64 0:14.5.2-ce.0.el7
  
Complete!
</pre>
</details>

6. Restart redis:
```sudo gitlab-ctl restart redis```

7. Check GitLab status:
```gitlab-ctl status```

<details>
  <summary>Expected output</summary>
   <pre>
run: alertmanager: (pid 539) 346s; run: log: (pid 1219) 593983s
run: gitaly: (pid 615) 337s; run: log: (pid 1214) 593983s
run: gitlab-exporter: (pid 525) 347s; run: log: (pid 1209) 593983s
run: gitlab-workhorse: (pid 518) 348s; run: log: (pid 1207) 593983s
run: grafana: (pid 549) 345s; run: log: (pid 1210) 593983s
run: logrotate: (pid 565) 345s; run: log: (pid 1213) 593983s
run: nginx: (pid 571) 344s; run: log: (pid 1208) 593983s
run: node-exporter: (pid 578) 344s; run: log: (pid 1215) 593983s
run: postgres-exporter: (pid 531) 347s; run: log: (pid 1217) 593983s
run: postgresql: (pid 1220) 593983s; run: log: (pid 1212) 593983s
run: puma: (pid 584) 344s; run: log: (pid 1205) 593983s
run: redis: (pid 1922) 24s; run: log: (pid 1211) 593983s
run: redis-exporter: (pid 590) 343s; run: log: (pid 1218) 593983s
run: sidekiq: (pid 595) 343s; run: log: (pid 1216) 593983s
</pre>
</details>

8. Check if the GitLab website is accessible and if the version listed on the Admin Panel is the same as the one you just updated.

