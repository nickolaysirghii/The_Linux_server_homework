# The_Linux_server_homework
[ec2-user@ip-172-31-33-20 NIkolay]$ pwd
/opt/47_48_evening_b/NIkolay
[ec2-user@ip-172-31-33-20 NIkolay]$ ls
script.sh  sleeper_2.sh  sleeper.sh
[ec2-user@ip-172-31-33-20 NIkolay]$ cat sleeper.sh
#!/bin/bash

for run in {1..10}
do
        echo "I think that there are two ways to list the time on the screen . This is the first :"
date | cut -c12-19
echo "And this is the second :"
date +"%H:%M:%S"
ps -ef | wc -m
#sleep 5
sleep 0.5
done
[ec2-user@ip-172-31-33-20 NIkolay]$ cat sleeper_2.sh
Filesystem      Size  Used Avail Use% Mounted on
devtmpfs        474M     0  474M   0% /dev
tmpfs           483M     0  483M   0% /dev/shm
tmpfs           483M  648K  483M   1% /run
tmpfs           483M     0  483M   0% /sys/fs/cgroup
/dev/xvda1      8.0G  6.5G  1.6G  81% /
tmpfs            97M     0   97M   0% /run/user/1000
NAME="Amazon Linux"
"Amazon Linux"
[ec2-user@ip-172-31-33-20 NIkolay]$ cat script.sh
#!/bin/bash

df -h >> /opt/47_48_evening_b/NIkolay/sleeper_2.sh
cat /etc/os-release | head -1 >> sleeper_2.sh
cat /etc/os-release | head -1 | cut -c6-30 >> sleeper_2.sh


for TASK in {50..100}
do

        touch /opt/47_48_evening_b/NIkolay/$TASK.txt

done



[ec2-user@ip-172-31-33-20 NIkolay]$



