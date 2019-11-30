+++
title = "js Objects"
date = "2019-11-30"
pinned = false 
draft = false
image = "/img/jsObjects.png"
+++
<!-- OOP 
is a programming paradigm or a style of programming that is centered arround objects rather than functions
- What are the four core concepts in OOP?
1- Encapsulation: 
2- Abstructions
3- Inheritence
4- Polymorphism

properties are used to hold values
fnctions or methods are used to define some logics
Use object literals {} instead of new Object().

Use string literals "" instead of new String().

Use number literals 12345 instead of new Number().

Use boolean literals true / false instead of new Boolean().

Use array literals [] instead of new Array().

Use pattern literals /()/ instead of new RegExp().

Use function expressions () {} instead of new Function().
var x1 = {};            // new object
var x2 = "";            // new primitive string
var x3 = 0;             // new primitive number
var x4 = false;         // new primitive boolean
var x5 = [];            // new array object
var x6 = /()/           // new regexp object
var x7 = function(){};  // new function object
 -->
    In JAVASCRIPT almost everything is an object
- Booleans can be Objects ( if defined with the **new** keyword) `let bool = new Boolean(value) `
- Numbers can be Objects ( if defined with the **new** keyword) `let num = new Number(number)`
- Strings can be Objects ( if defined with teh **new** keyword) `let str = new String(string)`
- Dates are always objects
- Maths are always objectss
- Regular expressions are lalways objects
- Arrays are always objects
- Functions are always objects
* All Javascript values, except primitives, are objects.

    JavaScript Primitives
  - A primitive value is a value that has no properties or methods `let name = "chiar" `
  - A primitive data type is data that has a primitive value.

### Type of primitive Data Types:
* String
* Number
* Boolean 
* Null 
* undefined

## JavaScript Value vs Reference Types
- **Primitives** are copied by their `Value`
- **Objects** are copied by their `reference`

## Creating a JavaScript Object

* Define and ***create*** a single object, using an **object literal**.
  using properties(keys) and values
```js
let person = {
  firstName:"John",
  lastName:"Doe", 
  age:50, 
  eyeColor:"blue"
  };
```

* Define and ***create*** a single object, with the keyword **new**.
```js
let person = new Object(); // let person = new {}
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue";
```
    JavaScript Objects are Mutable: they are addressed by referencem not by vlaue
* Define an object ***Constructor***, and then create objects of the **Constructor** type
* In ECMAScript 5 `Object.create()` 

```js
// Constructor function for Person objects
function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}

// Create a Person object

let per = {
  first: "John",
  last : "Doe",
  age  : 22,
  eye  : "blue"
}
document.write("the new person is " + per.first + ".");
```