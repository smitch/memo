tcpdump -A port <port> -i <interface> dst <ipaddress> and/or src <ipaddress>

## [how to find tcp streams without final ack/fin sequence in a huge packet capture file](https://superuser.com/questions/402322/how-to-find-tcp-streams-without-final-ack-fin-sequence-in-a-huge-packet-capture)
```
tcpdump -r pcap-file 'tcp[tcpflags] & (tcp-syn|tcp-fin) > 0' | 
sed -r 's/^.*IP (.*) > (.*):.*$/\1 \2/'|sort|uniq -u
```

https://unix.stackexchange.com/questions/310854/tail-f-using-tcpdump-r

```
tail -c +1 -f /Path/to/syscontection.pcap | tcpdump -l -r -
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAxMTI4MDg0OV19
-->