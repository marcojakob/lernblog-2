+++
title = "Get starting with React"
date = "2019-08-29"
draft = false
pinned = false
image = "/img/react.png"
description = "Overview and start learning react"
+++
What Is React?

> React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called **Components**
>
> React has a few different kinds of components, but we’ll start with **React.Component** subclasses:

## 

```javascript
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}

// Example usage: <ShoppingList name="Mark" />
```

> The **render** method returns a  _description_ of what you want to see on the screen. React takes the description and displays the result. In particular, **render** returns a  _**React element**_ , which is a lightweight description of what to render.

# Introduction to React Elements: 

## Install Create a React App

* Create **React App** is a tool that will allow us to set up a React project without any build config which will also set up all dev packs including webpack etc..
* to get started with React App, all you need to do is **Install create-react-app** as a -g dependency using Npm
  \- `npm install -g create-react-app `
* To generate  **React Project** we use the comand `create-react-app "project name"`
  *  My first [**React App**](https://github.com/chiarabdy/react-ll) is linked down below which would be follwed by the [**Tutorial**](https://reactjs.org/tutorial/tutorial.html)****

* Create React **Elements**
  Call `React.createElement()` and describe its arguments.
  Use `ReactDOM.render()` to render an element to a page.
  Describe how we can build elements out of other React elements.
  Add child elements and nested child elements.
  Pass properties to an element.

**`import React from 'react';`**`
`

**`import logo from './logo.svg';`**`
`

**`import './App.css';`**

**`export default App;`**
