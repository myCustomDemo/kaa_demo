### How to build and launch project

Project contains kaa-node.deb package 0.9.0 version and edited templates
for it.
Located at ~/kaa/server/containers/docker. Also exposed 3306 port on mariadb instance to access from jdbc in tests.

```
cd ~/kaa/server/containers/docker
./build.sh
cd using-compose/
python launch-kaa.py mariadb-cassandra 3
```

### Access kaa admin page:

```
http://localhost:8080/
```

### Issue on login page
```
500 Server Error The call failed on the server; see server log for details
```

This issue apperas only today on my linux pc. On OSX I can access kaa admin page.
Probably bug?