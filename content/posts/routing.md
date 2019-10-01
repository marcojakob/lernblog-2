+++
title = "Basic Routing"
date = "2019-10-01"
pinned = false
draft = false
img = "/img/nodejs.png"
+++
## Routing
Routing defines the way in which the client requests are handled by the application endpoints.
### Implementation of routing in Node.js: 
There are two ways to implement routing in node.js which are listed below:
* Routing with Express

    __Express.js has an “app” object corresponding to HTTP. We define the routes by using the methods of this “app” object. This app object specifies a callback function, which is called when a request is received. We have different methods in app object for a different type of request.__
> will talk about express in comming posts.

* Without using Framework
```js
const http = require('http');
const fs = require('fs');

const server = http.createServer((req,res)=>{
console.log('request was made: ' + req.url);
if(req.url === '/home' || req.url === '/'){
    res.writeHead(200, {'Content-Type'});
    fs.createReadStream(__dirname + '/index.html').pipe(res);
}
})
server.listen(3000, '127.0.0.1');
console.log('Listining to port 3000');
```