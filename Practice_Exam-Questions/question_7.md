### **Q. Synchronize time of your system with the server classroom.example.com**
### Answer :-
```
[root@localhost ~]# yum install -y chronyd

[root@localhost ~]# systemctl start chronyd

[root@localhost ~]# systemctl enable chronyd

[root@localhost ~]# vim /etc/chrony.d

in this configuration file comment active server and add given server

add --> server classroom.example.com iburst

save changes

[root@localhost ~]# systemctl restart chronyd
```