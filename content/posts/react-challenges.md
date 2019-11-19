+++
title = "React Challenges"
date = "2019-09-05"
draft = false
pinned = false
image = "/img/react.png"
+++

## 1- React: Create a Simple JSX Element 
### Instructions: 
    element and add the text Hello JSX! inside it. 
[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch000.jsx)

The current code uses **JSX** to assign a div element to the constant JSX. Replace the div with an h1 element and add the text Hello JSX! inside it. 
[SULUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch000.jsx)

## 1- React: Create a Simple JSX Element

#### Instructions:

# List of Reacht exercises
## 1- React: Create a Simple JSX Element 
#### Instructions: 
     element and add the text Hello JSX! inside it. 
[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch000.jsx)

The current code uses **JSX** to assign a div element to the constant JSX. Replace the div with an h1 element and add the text Hello JSX! inside it. 
[SULUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch000.jsx)

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

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch001.jsx)

* The constant JSX should return a div element.
* The div should contain a p tag as the second element.
* The div should contain a ul tag as the third element.
* The div should contain an h1 tag as the first element.
* The ul should contain three li elements.
    [SOULUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch001.jsx)

## 3- React: Add Comments in JSX

JSX is a syntax that gets compiled into valid JavaScript. Sometimes, for readability, you might need to add comments to your code. Like most programming languages, JSX has its own way to do this.

To put comments inside JSX, you use the syntax {/\* \*/}to wrap around the comment text.

The code editor has a JSX element similar to what you created in the last challenge. Add a comment somewhere within the provided divelement, without modifying the existing h1or pelements.

### Instructions:

    * The constant JSXshould return a divelement.
    * The divshould contain an h1tag as the first element.
    * The divshould contain a ptag as the second element.
    * The JSXshould include a comment.

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch002.jsx)

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

  [SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch003.jsx)

## 5- React: Define an HTML Class in JSX
Apply a class of myDivto the divprovided in the JSX code.

    * The constant JSXshould return a divelement.
    * The divhas a class of myDiv.
[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch004.jsx)

## 6- React: Learn About Self-Closing JSX Tags
Fix the errors in the code editor so that it is valid JSX and successfully transpiles. Make sure you don't change any of the content - you only need to close tags where they are needed.

    * The constant JSXshould return a divelement.
    * The divshould contain a brtag.
    * The divshould contain an hrtag.

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch005.jsx)
## 7- React: Create a Stateless Functional Component
The code editor has a function called MyComponent. Complete this function so it returns a single divelement which contains some string of text.
Note: The text is considered a child of the divelement, so you will not be able to use a self-closing tag.
### Instructions:

    * MyComponentshould return JSX.
    * MyComponentshould return a divelement.
    * The divelement should contain a string of text.

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch006.jsx)
## 8- React: Create a React Component
The other way to define a React component is with the ES6 classsyntax
### Instructions:
MyComponentis defined in the code editor using class syntax. Finish writing the rendermethod so it returns a divelement that contains an h1with the text Hello React!.

    * The React component should return a divelement.
    * The returned divshould render an h1header within it.
    * The h1header should contain the string Hello React!.

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch007.jsx)

## 9- React: Create a Component with Composition
 we can compose multiple React components together. Imagine you are building an App and have created three components, a **Navbar**, **Dashboard**, and **Footer**. To compose these components together, you could create an **App** parent component which renders each of these three components as children. To render a component as a child in a React component, you include the component name written as a custom HTML tag in the JSX. For example, in the **render** method you could write:

### Instructions
In the code editor, there is a simple functional component called ChildComponent and a class component called ParentComponent. Compose the two together by rendering the ChildComponent within the ParentComponent. Make sure to close the ChildComponent tag with a forward slash. Note: ChildComponent is defined with an ES6 arrow function because this is a very common practice when using React. However, know that this is just a function. If you aren't familiar with the arrow function syntax, please refer to the JavaScript section.

    * The React component should return a single divelement.
    * The component should return two nested elements.
    * The component should return the ChildComponent as its second child  

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch008.jsx)

## 10 - React: Use React to Render Nested Components

The last challenge showed a simple way to compose two components, but there are many different ways you can compose components with React.

Component composition is one of React's powerful features. When you work with React, it is important to start thinking about your user interface in terms of components like the App example in the last challenge. You break down your UI into its basic building blocks, and those pieces become the components. This helps to separate the code responsible for the UI from the code responsible for handling your application logic. It can greatly simplify the development and maintenance of complex projects.


There are two functional components defined in the code editor, called TypesOfFruitand Fruits. Take the TypesOfFruitcomponent and compose it, or nest it, within the Fruitscomponent. Then take the Fruitscomponent and nest it within the TypesOfFoodcomponent. The result should be a child component, nested within a parent component, which is nested within a parent component of its own!
### Instructions
    * The TypesOfFoodcomponent should return a single divelement.
    * The TypesOfFoodcomponent should return the Fruitscomponent.
    * The Fruitscomponent should return the TypesOfFruitcomponent.
    * The TypesOfFruitcomponent should return the h2and ulelements.

[SOLUTIONS](https://github.com/chiarabdy/lernblogTesting/blob/master/content/challenges/react/ch009.jsx)

