+++
title = "react-chalanges"
date = "2019-09-05"
draft = false
pinned = true
image = "/img/react.png"
+++

# What is JSX?
 * JSX stands for JavaScript XML.

 * JSX allows us to write HTML in React.

 * JSX makes it easier to write and add HTML in React.

## Coding JSX
JSX allows us to write HTML elements in JavaScript and place them in the DOM without any createElement()  and/or appendChild()  methods.

JSX converts HTML tags into react elements.

You are not required to use JSX, but JSX makes it easier to write React applications.

Let us demonstrate with two examples, the first uses JSX and the second does not:

Example 1
JSX:
~~~
const myelement = <h1>I Love JSX!</h1>;
ReactDOM.render(myelement, document.getElementById('root'));
~~~