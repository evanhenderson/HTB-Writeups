add blocky.htb to etc/hosts

then run gobuster

~~~
gobuster dir -u "http://blocky.htb" -w "/usr/share/wordlists/dirb/small.txt"
===============================================================
Gobuster v3.1.0
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://blocky.htb
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/dirb/small.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.1.0
[+] Timeout:                 10s
===============================================================
2024/03/28 05:14:52 Starting gobuster in directory enumeration mode
===============================================================
/javascript           (Status: 301) [Size: 313] [--> http://blocky.htb/javascript/]
Progress: 531 / 960 (55.31%)                                                    Progress: 601 / 960 (62.60%)                                                    /phpmyadmin           (Status: 301) [Size: 313] [--> http://blocky.htb/phpmyadmin/]
Progress: 671 / 960 (69.90%)                                                    Progress: 741 / 960 (77.19%)                                                    Progress: 811 / 960 (84.48%)                                                    Progress: 871 / 960 (90.73%)                                                    Progress: 941 / 960 (98.02%)                                                                                                                                       
===============================================================
2024/03/28 05:15:02 Finished
===============================================================

~~~

found /phpmyadmin