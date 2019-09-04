+++
title = "React ES6"
date = "2019-09-04"
draft = false
pinned = false
image = "/img/es6-react.jpg"
+++
# What is ES6?

* ES6 stands for ECMAScript 6.
* ECMAScript was created to standardize JavaScript, and ES6 is the 6th version of ECMAScript, it was published in 2015, and is also known as ECMAScript 2015.

## Why ES6 with React?

* React uses ES6, and you should be familiar with some of the new features like:
  > Classes
  > Arrow Functions
  > Variables(let, const, var)

## Classes

_ES6 introduced classes._

> A class is a type of function, but instead of using the keyword function to initiate it, we use the keyword class, and the properties is assigned inside aconstructor() method.

* A simple class constructor:


```
class Car {

constructor(name) {

this.brand = name;

}}
```

## Method in Classes

> a method is a function that belongs to a class. In JavaScript, however, amethod is a function that belongs to an object. Everything in JavaScript is an object; a function is an object; an Array is an object

**You can add your own methods in a class:**

***Example***

### Create a method named "present":
~~~
class Car {
   constructor(name) {
     this.brand = name;
   }

   present() {
     return 'I have a ' + this.brand;
   }
}
mycar = new Car("Ford");
mycar.present();
~~~

 ## Class Inheritance
 > To create a class inheritance, use the ***extends*** keyword.
A class created with a class inheritance inherits all the methods from another class:

## Example
### Create a class named "Model" which will inherit the methods from the "Car" class:
~~~
class Car {
constructor(name) {
this.brand = name;
}

present() {
return 'I have a ' + this.brand;
}}

class Model extends Car {
constructor(name, mod) {
super(name);
this.model = mod;
}
show() {
return this.present() + ', it is a ' + this.model
}}
mycar = new Model("Ford", "Mustang");
mycar.show();
~~~
 > The super() method refers to the parent class.
By calling the super() method in the constructor method, we call the parent's constructor method and gets access to the parent's properties and methods.

## Syntax differencesFirst
 > let’s explore the syntax differences by looking at two code examples and annotating 
### them.React.createClass
 > Here we have a const with a React class assigned, with the important render function following on to complete a typical base component definition.
~~~
import React from 'react';

const Contacts = React.createClass({
render() {
return (
<div></div>
);
}});

export default Contacts;
~~~

### React.Component
 > Let’s take the above React.createClass definition and convert it to use an ES6 class.
~~~
import React from 'react';

class Contacts extends React.Component {
constructor(props) {
super(props);
}
render() {
return (
<div></div>
);
}}

export default Contacts;
~~~

