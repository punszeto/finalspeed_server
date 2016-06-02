finalspeed
========

esay install
----
```
wget  https://raw.githubusercontent.com/punszeto/finalspeed_server/master/install_fs.sh
chmod +x install_fs.sh
./install_fs.sh 2>&1 | tee install.log
```

about command 
---
```
check run and view log: tail -f /fs/server.log
uninstall: sh /fs/stop.sh ; rm -rf /fs
stop sh /fs/stop.sh
restart sh /fs/restart.sh; tail -f /fs/server.log
```

setting start 
--- 
```
chmod +x /etc/rc.local
vi /etc/rc.local
add
sh /fs/start.sh
```
setting auto restart
---
```
crontab -e
add
0 3 * * * sh /fs/restart.sh
```


Enjoy it! thx!!
 


