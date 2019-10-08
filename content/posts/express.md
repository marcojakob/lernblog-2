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
app.get('/',  (req, res)=> {
  res.send('Hello World!')
})
```
__Respond to POST request on the root route (/), the application’s home page:__
```js
app.post('/',  (req, res)=> {
  res.send('Got a POST request')
})
```
__Respond to a PUT request to the /user route:__

```js
app.put('/user',  (req, res)=> {
  res.send('Got a PUT request at /user')
})
```
__Respond to a DELETE request to the /user route:__
```js
app.delete('/user',  (req, res)=> {
  res.send('Got a DELETE request at /user')
})

```
## Route Methods
A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

The following code is an example of routes that are defined for the GET and the POST methods to the root of the app.
```js
// GET method route
app.get('/', (req, res)=> {
  res.send('GET request to the homepage')
})

// POST method route
app.post('/', (req, res)=> {
  res.send('POST request to the homepage')
})
```
**Express** supports methods that correspond to all **HTTP request methods**: ***get, post, and so on.*** For a full list,  [app.METHOD.](https://expressjs.com/en/4x/api.html#app.METHOD)

There is a special routing method, [app.all()](https://expressjs.com/en/4x/api.html#app.all), used to load middleware functions at a path for all HTTP request methods. **For example**, the following handler is executed for requests to the route ```“/secret”``` whether using ***GET, POST, PUT, DELETE,*** or any other HTTP request method supported in the http module.
```js
app.all('/secret',  (req, res, next) {
  console.log('Accessing the secret section ...')
  next() // pass control to the next handler
})
```
## Route Paths
Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.

The characters ?, +, *, and () are subsets of their regular expression counterparts. The hyphen (-) and the dot (.) are interpreted literally by string-based paths.

If you need to use the dollar character ($) in a path string, enclose it escaped within ([ and ]). For example, the path string for requests at “/data/$book”, would be “/data/([\$])book”.
### Examples
__This route path will match requests to the root route, /.__
```js
app.get('/',  (req, res)=> {
  res.send('root')
})
```
__This route path will match requests to /about.__
```j
app.get('/about',  (req, res)=> {
  res.send('about')
})
```
__This route path will match requests to /random.text.__
```js
app.get('/random.text',  (req, res)=> {
  res.send('random.text')
})
```
### Here are some examples of route paths based on string patterns.

__This route path will match acd and abcd.__
```js
app.get('/ab?cd',  (req, res)=> {
  res.send('ab?cd')
})
```
__This route path will match abcd, abbcd, abbbcd, and so on.__
```js
app.get('/ab+cd',  (req, res)=> {
  res.send('ab+cd')
})
```
__This route path will match abcd, abxcd, abRANDOMcd, ab123cd, and so on.__
```js
app.get('/ab*cd',  (req, res)=> {
  res.send('ab*cd')
})
```
__This route path will match /abe and /abcde.__
```js
app.get('/ab(cd)?e',  (req, res)=> {
  res.send('ab(cd)?e')
})
```
### Examples of route paths based on regular expressions:

__This route path will match anything with an “a” in it.__
```js
app.get(/a/,  (req, res)=> {
  res.send('/a/')
})
```
__This route path will match butterfly and dragonfly, but not butterflyman, dragonflyman, and so on.__
```js
app.get(/.*fly$/,  (req, res)=> {
  res.send('/.*fly$/')
})
```