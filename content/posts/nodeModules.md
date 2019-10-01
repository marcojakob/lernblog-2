+++
title = "Node Modules"
date = "2019-09-25"
draft = false
pinned = false
image = "/img/global-object.jpg"
+++
# Node.js Modules
A set of functions we want to include in our application.

## Built-in Modules
Node.js has a set of built-in modules which you can use without any further installation.
* Hier is a set of [Build-in Modules Reference in W3 Schools](https://www.w3schools.com/nodejs/ref_modules.asp)
* More about Node Modules in [Node.js main Website](https://nodejs.org/api/modules.html) 
## include Modules
To include a module, use the **require()** function with the name of the module:

```javascript
var http = require('http');
```
> Now your application has access to the HTTP module, and is able to create a server:
```javascript
http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html'});
  res.end('Hello World!');
}).listen(8080);
```
## require()
require function is the easiest way to include modules that exist in **separate files**. The basic functionality of require is that it reads a javascript file, executes the file, and then proceeds to return the exports object. An example module:
**Example**
> in count.js which is a Module, I've created a counter function.
In which applied to module.exports to the counter() to make it accessible outside of the module wherever we require that module
```javascript
var counter = function(arr){
    return `There are ${arr.length} Elements in this array`
[//]: # (template string uses ``(backticks) so that we can embed Variables
or expressions without concatenating them)
};
module.exports = counter; 
```
> Require it in app.js by setting the exports object to a the counter function or new object by using the **module.exports** object

```javascript
var counter = require('./count');

console.log(counter(["One", "Two", "Three"]));
```

## Module Patterns
Here is some different Module Patterns

### First
in stuff.js we have different Variables to be explored
```javascript
var counter = function(arr){
    return `There are ${arr.length} Elements in this array`
};

var adder = function (a,b){
  return `The sum of the 2 nubers is ${a+b}`;
}

var pi = 2.22;

module.exports.counter = counter; 
module.exports.adder = adder; 
module.exports.pi = pi; 
```
Those three objects are exported and available outside of the module where require it in app.js
To access them:

```javascript
var counter = require('./stuffs');

console.log(stuffs.counter(["One", "Two", "Three"]));
console.log(stuffs.adder(2,3));
console.log(stuffs.adder(stuff.pie,5));
```
### Second

```javascript
module.exports.counter = function(arr){
    return `There are ${arr.length} Elements in this array`
};

module.exports.adder = function (a,b){
  return `The sum of the 2 nubers is ${a+b}`;
}

module.exports.pi = 2.22;
```
### Finally

```javascript
var counter = function(arr){
    return `There are ${arr.length} Elements in this array`
};

var adder = function (a,b){
  return `The sum of the 2 nubers is ${a+b}`;
}

var pi = 2.22;

module.exports = {
  counter : counter,
  adder : adder,
  pi: pi
};
```
