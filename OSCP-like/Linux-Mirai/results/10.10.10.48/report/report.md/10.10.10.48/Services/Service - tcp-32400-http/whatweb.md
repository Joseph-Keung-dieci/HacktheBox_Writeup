```bash
whatweb --color=never --no-errors -a 3 -v http://10.10.10.48:32400 2>&1
```

[/home/parallels/HacktheBox/OSCP-like/Linux-Mirai/results/10.10.10.48/scans/tcp32400/tcp_32400_http_whatweb.txt](file:///home/parallels/HacktheBox/OSCP-like/Linux-Mirai/results/10.10.10.48/scans/tcp32400/tcp_32400_http_whatweb.txt):

```
WhatWeb report for http://10.10.10.48:32400
Status    : 401 Unauthorized
Title     : Unauthorized
IP        : 10.10.10.48
Country   : RESERVED, ZZ

Summary   : Script, UncommonHeaders[x-plex-protocol,x-plex-content-original-length,x-plex-content-compressed-length]

Detected Plugins:
[ Script ]
	This plugin detects instances of script HTML elements and
	returns the script language/type.


[ UncommonHeaders ]
	Uncommon HTTP server headers. The blacklist includes all
	the standard headers and many non standard but common ones.
	Interesting but fairly common headers should have their own
	plugins, eg. x-powered-by, server and x-aspnet-version.
	Info about headers can be found at www.http-stats.com

	String       : x-plex-protocol,x-plex-content-original-length,x-plex-content-compressed-length (from headers)

HTTP Headers:
	HTTP/1.1 401 Unauthorized
	Content-Type: text/html
	X-Plex-Protocol: 1.0
	Content-Encoding: gzip
	X-Plex-Content-Original-Length: 193
	X-Plex-Content-Compressed-Length: 157
	Content-Length: 157
	Cache-Control: no-cache
	Date: Sun, 18 Sep 2022 05:13:45 GMT



```
