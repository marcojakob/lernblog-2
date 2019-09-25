+++
title = "Global Objects"
date = "2019-09-25"
drift = false
pinned = false
image = "/img/global-object.jpg"
+++
# The Global Object
A global object is an object that always exists in the global scope.

In JavaScript, there's always a global object defined. In a web browser, when scripts create global variables, they're created as members of the global object. (In Node.js this is not the case.) The global object's interface depends on the execution context in which the script is running. For example:

* In a web browser, any code which the script doesn't specifically start up as a background task has a Window as its global object. This is the vast majority of JavaScript code on the Web.
* Code running in a Worker has a WorkerGlobalScope object as its global object.
* Scripts running under Node.js have an object called global as their global object.
Here is a list of [Global Object](https://nodejs.org/api/globals.html) in Node.js

### setTimeOut

~~~
setTimeout (function(){
console.log("3 Seconds have passed");
}, 3000);
~~~

### setInterval

~~~
var time = 0;
setInterval (function(){
    time += 2;
    console.log(time + ' Seconds have passed');
}, 2000);
~~~
###  clearInterval
~~~
var time = 0;

var timer = setInterval (function(){
    time += 2;
    console.log(time + ' Seconds have passed');
    if (timer >= 6){
        clearInterval(timer);
    }
}, 2000);

~~~
### __dirname
~~~
console.log(__dirname);
~~~

### __filename
~~~
console.log(__filename);
~~~
### 