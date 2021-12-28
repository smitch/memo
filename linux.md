# add user
useradd <user name>

# set password
passwd <user name>

# add user to sudoers(centos 6)
visudo
// add line below
// <usr name>   ALL=(ALL)       ALL

# inhibit root ssh login
 vi /etc/ssh/sshd_config
 PermitRootLogin no
 
 # set hostname
 hostname <hostname>
 vi /etc/sysconfig/network
 HOSTNAME=<hostname>
 vi /etc/hosts
 <ip address> <hostname>
 
# network
-  https://qiita.com/routerman/items/4d19b3084fa58723830c
```
# ip address add 192.168.11.100/24 dev eth0
# ip link set eth0 up
# echo "nameserver 192.168.11.1" >> resolv.conf
# echo "nameserver 8.8.8.8" >> resolv.conf
```

# htop
- https://sys-guard.com/post-6318/

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM3MjI2NjI2MCw3Mzc5MzI0NjUsMTg1OD
I3MjA0NV19
-->