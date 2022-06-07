---
layout: page
permalink: /cmd/
title: Useful commands. 
description: Useful commands for linux system. 
nav: false
nav_order: 2
---

## Giving writing permission to a user.

`sudo setfacl -m u:yisong:rwx yisong`

[https://askubuntu.com/questions/487527/give-specific-user-permission-to-write-to-a-folder-using-w-notation](https://askubuntu.com/questions/487527/give-specific-user-permission-to-write-to-a-folder-using-w-notation)


## Check disk usage. 

wing.nus@sle:/data3$ `df -h`
Filesystem      Size  Used Avail Use% Mounted on
udev             94G     0   94G   0% /dev
tmpfs            19G  2.4M   19G   1% /run
/dev/nvme0n1p1  822G  771G  9.6G  99% /
tmpfs            94G   99M   94G   1% /dev/shm
tmpfs           5.0M     0  5.0M   0% /run/lock
tmpfs            94G     0   94G   0% /sys/fs/cgroup
/dev/sda1       1.8T  627G  1.1T  37% /data
/dev/sdc1       1.9T  1.5T  408G  79% /data3
/dev/sdb1       1.9T  1.9T   11G 100% /data2



