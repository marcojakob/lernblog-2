+++
title = "React Challenges"
date = "2019-09-05"
draft = false
pinned = true
image = "/img/react.png"
+++
## 1- React: Create a Simple JSX Element 
### Instructions: 
    element and add the text Hello JSX! inside it. 
[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/ch000.jsx)

The current code uses **JSX** to assign a div element to the constant JSX. Replace the div with an h1 element and add the text Hello JSX! inside it. 
[SULUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/ch000.jsx)

## 2-React: Create a Complex JSX Element

### Instructions:

Define a new constant JSX that renders a div which contains the following elements in order:

An h1, a p, and an unordered list that contains three li items. You can include any text you want within each element.

Note: When rendering multiple elements like this, you can wrap them all in parentheses, but it's not strictly required. Also notice this challenge uses a div tag to wrap all the child elements within a single parent element. If you remove the div, the JSX will no longer transpile. Keep this in mind, since it will also apply when you return JSX elements in React components.

    * The constant JSX should return a div element.
    * The div should contain a p tag as the second element.
    * The div should contain a ul tag as the third element.
    * The div should contain an h1 tag as the first element.
    * The ul should contain three li elements.

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/ch001.jsx)

* The constant JSX should return a div element.
* The div should contain a p tag as the second element.
* The div should contain a ul tag as the third element.
* The div should contain an h1 tag as the first element.
* The ul should contain three li elements.
    [SOULUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/ch001.jsx)

## 3- React: Add Comments in JSX

JSX is a syntax that gets compiled into valid JavaScript. Sometimes, for readability, you might need to add comments to your code. Like most programming languages, JSX has its own way to do this.

To put comments inside JSX, you use the syntax {/\* \*/}to wrap around the comment text.

The code editor has a JSX element similar to what you created in the last challenge. Add a comment somewhere within the provided divelement, without modifying the existing h1or pelements.

### Instructions:

    * The constant JSXshould return a divelement.
    * The divshould contain an h1tag as the first element.
    * The divshould contain a ptag as the second element.
    * The JSXshould include a comment.
[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/ch002.jsx)

## 4- React: Render HTML Elements to the DOM
So far, you've learned that JSX is a convenient tool to write readable HTML within JavaScript. With React, we can render this JSX directly to the HTML DOM using React's rendering API known as ReactDOM.

ReactDOM offers a simple method to render React elements to the DOM which looks like this: ReactDOM.render(componentToRender, targetNode), where the first argument is the React element or component that you want to render, and the second argument is the DOM node that you want to render the component to.

As you would expect, ReactDOM.render()must be called after the JSX element declarations, just like how you must declare variables before using them.


The code editor has a simple JSX component. Use the ReactDOM.render()method to render this component to the page. You can pass defined JSX elements directly in as the first argument and use document.getElementById()to select the DOM node to render them to. There is a divwith id='challenge-node'available for you to use. Make sure you don't change the JSXconstant.
### Instructions:
    * The constant JSXshould return a divelement.
    * The divshould contain an h1tag as the first element.
    * The divshould contain a ptag as the second element.
    * The provided JSX element should render to the DOM node with id challenge-node.

  [SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/ch003.jsx)
