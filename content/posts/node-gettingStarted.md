+++
title = "getting started with Node,js "
date = "2019-09-25"
draft = false
pinned = true
image = "/img/nodejs.png"
+++
## NodeJS
    NodeJS is an open-source, cross-platform runtime environment for developing server-side web applications. NodeJS also has an event-driven architecture capable of asynchronous I/O.

    NodeJS uses an event-driven, non-blocking I/O model that makes it lightweight and efficient.
# Getting Started
create test.js file after setting up the environment which print Hello, World
and simply run it by typing
~~~
node test.js
~~~

~~~
var http = require('http');

http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html'});
  res.end('Hello World!');
}).listen(8080);
~~~
