
https://serverfault.com/questions/654293/snmp-snmpwalk-does-not-return-textual-oids

https://qiita.com/Mabuchin/items/d435c0afb4f0ca17ad25
```
snmpwalk -Os -M /volume/~/mibs -m all tp1 public .1.3.6.1.2.1.4
```

```
snmpwalk -M /usr/share/snmp/mibs:/usr/share/snmp/mibs/iana:/usr/share/snmp/mibs/ietf:./yamaha-private-mib -m all -v 2c -c <community> 192.168.100.2
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDAyMjk1NDc3LDE5NjcyOTQ5MTBdfQ==
-->