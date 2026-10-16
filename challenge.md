# Security Detective Challenge

## Question 1
**Question:** Which user are you logged in as, and where is your home folder?

**Answer:** I am logged in as noorulain027. My home folder is /home/lab5user.

**Commands:** `whoami`, `pwd`

## Question 2
**Question:** What is the server's name, and which Ubuntu version does it run?

**Answer:** My server name is lab5user. It runs 24.04.3 LTS.

**Commands:** `hostname`, `cat /etc/os-release`

## Question 3
**Question:** How much RAM does the server have, and how much disk space is free?

**Answer:** My server has 1.9Gi of total RAM. The available disk space on `/` is 893Mi.

**Commands:** `free -h`, `df -h /`

## Question 4
**Question:** Which users on this server can log in with /bin/bash?

**Answer:** The users listed by the following command have `/bin/bash` as their login shell: noorulain027.

**Command:** `grep '/bin/bash' /etc/passwd`

## Question 5
**Question:** How many processes are running right now?

**Answer:** The command returned 241 lines, including the header.

**Command:** `ps aux | wc -l`

## Question 6
**Question:** At what time was lab5user created, and at what time was it deleted?

**Answer:** The log shows Oct 16 07:12:17, Oct 16 7:13:32.

**Commands:** `sudo grep lab5user /var/log/auth.log`, `sudo journalctl | grep lab5user` (use the available log source)
