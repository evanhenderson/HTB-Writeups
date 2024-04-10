found /cgi-bin/ 
~~~
gobuster dir -u http://10.129.243.115 -w /usr/share/wordlists/dirb/small.txt -s 302,307,200,204,301,403
===============================================================
Gobuster v3.1.0
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://10.129.243.115
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/dirb/small.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.1.0
[+] Timeout:                 10s
===============================================================
2024/03/28 04:34:31 Starting gobuster in directory enumeration mode
===============================================================
/cgi-bin/             (Status: 403) [Size: 297]
Progress: 791 / 960 (82.40%)                  ^C
[!] Keyboard interrupt detected, terminating.
                                               
===============================================================
2024/03/28 04:34:37 Finished
===============================================================
~~~
run it again to look for files:

~~~
gobuster dir -u http://10.129.243.115/cgi-bin/ -w /usr/share/wordlists/dirb/small.txt -s 302,307,200,204,301,403 -x sh,pl
===============================================================
Gobuster v3.1.0
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://10.129.243.115/cgi-bin/
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/dirb/small.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.1.0
[+] Extensions:              sh,pl
[+] Timeout:                 10s
===============================================================
2024/03/28 04:36:25 Starting gobuster in directory enumeration mode
===============================================================
/user.sh              (Status: 200) [Size: 118]
                                               
===============================================================
2024/03/28 04:36:48 Finished
===============================================================

~~~
throw into burpsuite