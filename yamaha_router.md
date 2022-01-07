


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
Host 192.168.0.1
KexAlgorithms +diffie-hellman-group1-sha1
```
- https://lowreal.net/2021/10/01/1

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDQ2MzE4NTI2LDY1NTUyNjg0MywtMjU0OD
U3MjI0XX0=
-->