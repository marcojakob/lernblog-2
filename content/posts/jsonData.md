+++
title = 'Serving JSON Data'
date = '2019-10-01'
pinned = false
draft = false 
image = '/img/nodejs.png'
+++
## serving json to the client
__Send it th the response object directly by using the ```end()``` method__

```js
const http = require('http');
const fs = require('fs');
const port = 3000;

const server =  http.createServer((req,res)=>{
    res.writeHead(200, {'Content-Type': 'application/json'});
    const myObj = {
        name = 'Chiar',
        lastName = 'Abdi',
        age = 31
    };
        res.end(JSON.stringify(myobj));
    });
});

server.listen(port, (error)=>{
    if (error){
        console.log('Something Went wrong');
    } else {
        console.log('Server listining on port 3000');
    }
})
```