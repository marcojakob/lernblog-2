+++
title = "React Components"
date = "2019-09-02"
draft = false
pinned = false
image = "/img/download.png"
+++
# Overview

React lets you define components as _classes or functions_. Components defined as classes currently provide more features which are described in detail on this page. To define a React component class, you need to extend **React.Component**:

```
 class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

The only method you must define in a React.Component subclass is called **render()**. All the other methods described on this page are optional.

* All the components should be capitalised 

## The Component Lifecycle

> Each component has several “lifecycle methods” that you can override to run code at particular times in the process. You can use this lifecycle diagram as a cheat sheet. In the list below, commonly used lifecycle methods are marked as bold. The rest of them exist for relatively rare use cases.



![](/img/lifecycles.jpg)

I followed the tutorial with a Project which would be my old portfolio and later on it will be deployed and served with Github pages

* The project on [Github](https://github.com/chiarabdy/chiarabdy.github.io)
