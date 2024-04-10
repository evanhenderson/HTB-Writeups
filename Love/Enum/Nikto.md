port 5000:
~~~
- Nikto v2.1.6
---------------------------------------------------------------------------
+ Target IP:          10.129.48.103
+ Target Hostname:    10.129.48.103
+ Target Port:        80
+ Start Time:         2024-04-04 04:15:08 (GMT1)
---------------------------------------------------------------------------
+ Server: Apache/2.4.46 (Win64) OpenSSL/1.1.1j PHP/7.3.27
+ Retrieved x-powered-by header: PHP/7.3.27
+ The anti-clickjacking X-Frame-Options header is not present.
+ The X-XSS-Protection header is not defined. This header can hint to the user agent to protect against some forms of XSS
+ The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type
+ Cookie PHPSESSID created without the httponly flag
+ Web Server returns a valid response with junk HTTP methods, this may cause false positives.
+ OSVDB-877: HTTP TRACE method is active, suggesting the host is vulnerable to XST
+ OSVDB-3092: /admin/: This might be interesting...
+ OSVDB-3268: /includes/: Directory indexing found.
+ OSVDB-3092: /includes/: This might be interesting...
+ OSVDB-3093: /admin/index.php: This might be interesting... has been seen in web logs from an unknown scanner.
+ OSVDB-3268: /icons/: Directory indexing found.
+ OSVDB-3268: /images/: Directory indexing found.
+ OSVDB-3233: /icons/README: Apache default file found.
+ OSVDB-3092: /Admin/: This might be interesting...


~~~

ip:
~~~
- Nikto v2.1.6
---------------------------------------------------------------------------
+ Target IP:          10.129.48.103
+ Target Hostname:    10.129.48.103
+ Target Port:        80
+ Start Time:         2024-04-04 04:15:08 (GMT1)
---------------------------------------------------------------------------
+ Server: Apache/2.4.46 (Win64) OpenSSL/1.1.1j PHP/7.3.27
+ Retrieved x-powered-by header: PHP/7.3.27
+ The anti-clickjacking X-Frame-Options header is not present.
+ The X-XSS-Protection header is not defined. This header can hint to the user agent to protect against some forms of XSS
+ The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type
+ Cookie PHPSESSID created without the httponly flag
+ Web Server returns a valid response with junk HTTP methods, this may cause false positives.
+ OSVDB-877: HTTP TRACE method is active, suggesting the host is vulnerable to XST
+ OSVDB-3092: /admin/: This might be interesting...
+ OSVDB-3268: /includes/: Directory indexing found.
+ OSVDB-3092: /includes/: This might be interesting...
+ OSVDB-3093: /admin/index.php: This might be interesting... has been seen in web logs from an unknown scanner.
+ OSVDB-3268: /icons/: Directory indexing found.
+ OSVDB-3268: /images/: Directory indexing found.
+ OSVDB-3233: /icons/README: Apache default file found.
+ OSVDB-3092: /Admin/: This might be interesting...
+ 8724 requests: 0 error(s) and 15 item(s) reported on remote host
+ End Time:           2024-04-04 04:28:44 (GMT1) (816 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested

~~~