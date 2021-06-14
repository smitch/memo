tcpdump -A port <port> -i <interface> dst <ipaddress> and/or src <ipaddress>

## [how to find tcp streams without final ack/fin sequence in a huge packet capture file](https://superuser.com/questions/402322/how-to-find-tcp-streams-without-final-ack-fin-sequence-in-a-huge-packet-capture)
```
tcpdump -r pcap-file 'tcp[tcpflags] & (tcp-syn|tcp-fin) > 0' | 
sed -r 's/^.*IP (.*) > (.*):.*$/\1 \2/'|sort|uniq -u
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjU0NDYxNDk5XX0=
-->