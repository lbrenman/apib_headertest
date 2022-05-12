# An API Builder project to see how to read and set custom headers in an API

See [**blog post**](https://gist.github.com/lbrenman/c66505f124eb58e1f166ae6354527ef0) for details

Call API:

```
curl -is -H "accept: application/json" -H "x-customheader: aaa" -X GET "http://localhost:8080/api/user"
```

Response:

```
HTTP/1.1 200 OK
x-xss-protection: 1; mode=block
x-frame-options: DENY
surrogate-control: no-store
cache-control: no-store, no-cache, must-revalidate, proxy-revalidate
pragma: no-cache
expires: 0
x-content-type-options: nosniff
server: API Builder/4.89.0
request-id: c5bdf1d0-130b-42b7-bf75-965847a22b5b
start-time: 1652389384455
x-anothercustomheader: aaa,1234
content-type: application/json; charset=utf-8
response-time: 3
content-length: 9
Vary: Accept-Encoding
Date: Thu, 12 May 2022 21:03:04 GMT
Connection: keep-alive
Keep-Alive: timeout=5

"success"	
```
