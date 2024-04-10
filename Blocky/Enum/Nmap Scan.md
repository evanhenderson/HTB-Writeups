
~~~
nmap -sC -sV 10.129.243.80
Starting Nmap 7.93 ( https://nmap.org ) at 2024-03-28 04:49 GMT
Nmap scan report for 10.129.243.80
Host is up (0.075s latency).
Not shown: 996 filtered tcp ports (no-response)
PORT     STATE  SERVICE VERSION
21/tcp   open   ftp?
22/tcp   open   ssh     OpenSSH 7.2p2 Ubuntu 4ubuntu2.2 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   2048 d62b99b4d5e753ce2bfcb5d79d79fba2 (RSA)
|   256 5d7f389570c9beac67a01e86e7978403 (ECDSA)
|_  256 09d5c204951a90ef87562597df837067 (ED25519)
80/tcp   open   http    Apache httpd 2.4.18
|_http-title: Did not follow redirect to http://blocky.htb
|_http-server-header: Apache/2.4.18 (Ubuntu)
8192/tcp closed sophos
Service Info: Host: 127.0.1.1; OS: Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 239.24 seconds

~~~
udp scan
~~~
sudo nmap -sU 10.129.243.80
Starting Nmap 7.93 ( https://nmap.org ) at 2024-03-28 04:49 GMT
Nmap scan report for 10.129.243.80
Host is up (0.072s latency).
Not shown: 998 open|filtered udp ports (no-response)
PORT   STATE  SERVICE
22/udp closed ssh
80/udp closed http

Nmap done: 1 IP address (1 host up) scanned in 12.50 seconds

~~~