+++
title = "HTTP"
date = "2019-09-30"
pinned = false
draft = false
image = "img/http.jpg"
+++
## HTTP
is a Node.js built-in module, which allows Node.js to transfer data over the Hyper Text Transfer Protocol (HTTP).

* To include the HTTP module, use the ```require()``` method:
* To use the HTTP server and client one must 

```js
require('http')
```
__HTTP message headers are represented by an object like this:__
```js
{ 'content-length': '123',
  'content-type': 'text/plain',
  'connection': 'keep-alive',
  'host': 'mysite.com',
  'accept': '*/*' }
  ```
## SERVER

_The **HTTP module** can create an **HTTP server** that listens to server ports and gives a response back to the client.
Use the ```createServer()``` method to create an **HTTP server**:_
```js
const http = require('http');

//create a server object:
http.createServer(function (req, res) {
  res.write('Hello World!'); //write a response to the client
  res.end(); //end the response
}).listen(8080); //the server object listens on port 8080
```
## Add an HTTP Header
If the response from the **HTTP server** is supposed to be displayed as HTML, you should include an **HTTP header** with the correct content type:
```js
var http = require('http');
http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html'});
  res.write('Hello World!');
  res.end();
}).listen(8080);
```
