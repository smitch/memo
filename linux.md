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
 
