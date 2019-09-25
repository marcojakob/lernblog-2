+++
title = "Node.js Event Module"
date = "2019-09-25"
draft = false
pinned = true
image = "/img/eventModule.jpg"
+++
# Built-in Modules
## Event
>The Events module provides a way of working with events.
In Node.js, all events are an instance of the **EventEmitter** object

### Syntax
    The syntax for including the Events module, and creating an EventEmitter in your application:
~~~
var events = require('events');
var eventEmitter = new events.EventEmitter();
~~~
### EventEmitter Properties and Methods
| Module| Description|       
--- | ---
|addListener()| Adds the specified listener|
|defaultMaxListeners	|Sets the maximum number of listeners allowed for one event. Default is 10|
|emit()	|Call all the listeners registered with the specified name|
|eventNames()	|Returns an array containing all registered events|
|getMaxListeners()	|Returns the maximum number of listeners allowed for one event|
|listenerCount()	|Returns the number of listeners with the specified name|
|listeners()	|Returns an array of listeners with the specified name|
|on()	|Adds the specified listener|
|once()	|Adds the specified listener once. When the specified listener has been executed, the listener is removed|
|prependListener()	|Adds the specified listener as the first event with the specified name
|prependOnceListener()	|Adds the specified listener as the first event with the specified name, once. When the specified |
|listener has been |executed, the listener is removed|
|removeAllListeners()	|Removes all listeners with the specified name, or ALL listeners if no name is specified|
|removeListener()	|Removes the specified listener with the specified name|
|setMaxListeners()	|Sets the maximum number of listeners allowed for one event. Default is 10|
