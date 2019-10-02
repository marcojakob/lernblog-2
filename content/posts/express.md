+++
title = "Express Basic Routing"
date = "2019-10-01"
pinned = false
draft = false
image = "/img/expressjs.png"
+++
## Routing: 
refers to determining how an application responds to a client request to a particular endpoint, which is a URI (or path) and a specific HTTP request method (GET, POST, and so on).

Each route can have one or more handler functions, which are executed when the route is matched.

Route definition takes the following structure:
```js
app.METHOD(PATH, HANDLER)
```
### Where:

* app is an instance of express.
* METHOD is an HTTP request method, in lowercase.
* PATH is a path on the server.
* HANDLER is the function executed when the route is matched.

__The following examples illustrate defining simple routes.
Respond with Hello World! on the homepage:__
```js
app.get('/', function (req, res) {
  res.send('Hello World!')
})
```
__Respond to POST request on the root route (/), the application’s home page:__
```js
app.post('/', function (req, res) {
  res.send('Got a POST request')
})
```
__Respond to a PUT request to the /user route:__

```js
app.put('/user', function (req, res) {
  res.send('Got a PUT request at /user')
})
```
__Respond to a DELETE request to the /user route:__
```js
app.delete('/user', function (req, res) {
  res.send('Got a DELETE request at /user')
})

```
