


-  [デバッグログを確認する。](https://network.yamaha.com/setting/router_firewall/ts_router/server_release#point02)

```
syslog debug on
show log reverse
```

文字化け対策
```
cosole character ja.utf8
```


SSH設定

```
login user <user> <password>
sshd host key generate
sshd service on
```

```
Host 192.168.0.1
KexAlgorithms +diffie-hellman-group1-sha1
```
- https://lowreal.net/2021/10/01/1

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcxMDI4ODQzOF19
-->