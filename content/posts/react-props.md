+++
title = "React Props"
date = "2019-09-07"
draft = false
pinned = false
image = "/img/react.png"
+++

* Props are arguments passed into React components.
* Props are passed to components via HTML attributes.

* React Props are like function arguments in JavaScript and attributes in HTML.

To send props into a component, use the same syntax as HTML attributes:

**Example**
Add a "brand" attribute to the Car element:

~~~ 
const myelement = <Car brand="Ford" />;
~~~

The component receives the argument as a **props** object:

**Example**
Use the brand attribute in the component:
~~~
class Car extends React.Component {
  render() {
    return <h2>I am a {this.props.brand}!</h1>;
  }
}
~~~
## Pass Data
Props are also how you pass data from one component to another, as parameters.

**Example**
Send the "brand" property from the Garage component to the Car component:
~~~
class Car extends React.Component {
  render() {
    return <h2>I am a {this.props.brand}!</h2>;
  }
}

class Garage extends React.Component {
  render() {
    return (
      <div>
      <h1>Who lives in my garage?</h1>
      <Car brand="Ford" />
      </div>
    );
  }
}

ReactDOM.render(<Garage />, document.getElementById('root'));
~~~
    If we have a variable to send, and not a string as in the example above, we just put the variable name inside curly brackets:

**Example**
Create a variable named "carname" and send it to the Car component:
~~~
class Car extends React.Component {
  render() {
    return <h2>I am a {this.props.brand}!</h2>;
  }
}

class Garage extends React.Component {
  render() {
    const carname = "Ford";
    return (
      <div>
      <h1>Who lives in my garage?</h1>
      <Car brand={carname} />
      </div>
    );
  }
}

ReactDOM.render(<Garage />, document.getElementById('root'));
~~~
Or if it was an **object**:

**Example**
Create an object named "carinfo" and send it to the Car component:
~~~
class Car extends React.Component {
  render() {
    return <h2>I am a {this.props.brand.model}!</h2>;
  }
}

class Garage extends React.Component {
  render() {
    const carinfo = {name: "Ford", model: "Mustang"};
    return (
      <div>
      <h1>Who lives in my garage?</h1>
      <Car brand={carinfo} />
      </div>
    );
  }
}

ReactDOM.render(<Garage />, document.getElementById('root'));
~~~

## Props in the Constructor
    If your component has a constructor function, the props should always be passed to the constructor and also to the React.Component via the super() method.
        
**Example**
~~~
class Car extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return <h2>I am a Car!</h2>;
  }
}

ReactDOM.render(<Car model="Mustang"/>, document.getElementById('root'));
~~~
