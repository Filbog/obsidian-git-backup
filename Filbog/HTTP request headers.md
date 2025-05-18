03-11-2024

From ***Hypermedia Systems***:
individual lines of name/value pairs separated by a colon. The request headers provide _metadata_ that can be used by the server to determine exactly how to respond to the client request. For example, here's an HTTP request:
```
GET /book/contents/ HTTP/1.1
Accept: text/html,*/*
Host: hypermedia.systems
```
and a response to that HTTP request:
```
HTTP/1.1 200 OK
Content-Type: text/html; charset=utf-8
Content-Length: 870
Server: Werkzeug/2.0.2 Python/3.8.10
Date: Sat, 23 Apr 2022 18:27:55 GMT

<html lang="en">
<body>
  <header>
    <h1>HYPERMEDIA SYSTEMS</h1>
  </header>
  ...
</body>
</html>

```
After the first line, we have those headers. Then, we have the HTML content that comes in the response and will populate the browser window.
### Hashtags:
#hypermediasystems #coding #codingfundamentals 

### References (source material, similar notes):
