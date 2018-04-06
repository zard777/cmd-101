
 + **You have a new challenge!**
 + **access.log.1 and access.log.2 are http server logs.**
 + **Print the IP addresses common to both files, one per line.**


$ cat access.log.1
```
108.68.174.15 - - [09/Jan/2017:22:32:19 +0100] "GET /foo/create HTTP/1.0" 200 2477
17.2.20.139 - - [09/Jan/2017:22:33:48 +0100] "GET /posts/foo?appID=xxxx HTTP/1.0" 200 2477
28.151.137.59 - - [09/Jan/2017:22:37:57 +0100] "GET /foo/create HTTP/1.0" 200 1116
199.150.241.179 - - [09/Jan/2017:22:38:34 +0100] "GET /bar/create HTTP/1.0" 200 3240
2.71.250.27 - - [09/Jan/2017:22:41:26 +0100] "GET /pages/create HTTP/1.0" 500 2477
17.137.186.194 - - [09/Jan/2017:22:43:17 +0100] "GET /pages/create HTTP/1.0" 200 1116
151.84.119.34 - - [09/Jan/2017:22:47:51 +0100] "GET /posts/1/display HTTP/1.0" 404 3471
4.180.204.195 - - [09/Jan/2017:22:49:53 +0100] "GET /foo/create HTTP/1.0" 502 1116
9.230.96.54 - - [09/Jan/2017:22:52:58 +0100] "GET /bar/create HTTP/1.0" 200 1116
157.143.233.21 - - [09/Jan/2017:22:53:50 +0100] "GET /posts/foo?appID=xxxx HTTP/1.0" 502 1083
```
$ cat access.log.2
```
89.148.148.238 - - [09/Jan/2017:22:33:09 +0100] "GET /posts/1/display HTTP/1.0" 502 2477
12.135.14.52 - - [09/Jan/2017:22:35:28 +0100] "GET /pages/create HTTP/1.0" 404 3471
81.196.171.245 - - [09/Jan/2017:22:37:53 +0100] "GET /posts/2/display HTTP/1.0" 200 2497
202.141.16.141 - - [09/Jan/2017:22:42:48 +0100] "GET /pages/create HTTP/1.0" 200 2477
132.202.73.71 - - [09/Jan/2017:22:45:23 +0100] "PUT /posts/foo?appID=xxxx HTTP/1.0" 200 2497
89.169.186.129 - - [09/Jan/2017:22:49:29 +0100] "POST /pages/create HTTP/1.0" 200 1116
17.137.186.194 - - [09/Jan/2017:22:53:54 +0100] "GET /posts/foo?appID=xxxx HTTP/1.0" 200 3471
2.71.250.27 - - [09/Jan/2017:22:57:17 +0100] "POST /posts/foo?appID=xxxx HTTP/1.0" 404 1083
28.151.137.59 - - [09/Jan/2017:23:00:50 +0100] "GET /foo/create HTTP/1.0" 502 3471
108.68.174.15 - - [09/Jan/2017:23:03:35 +0100] "GET /posts/1/display HTTP/1.0" 200 2497
```

