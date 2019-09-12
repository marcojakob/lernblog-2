+++
title = "Getting started with VueJs"
date = "2019-09-12"
draft = false
pinned = false
image = "/img/vue-getting-started.jpg"
+++
# What is Vue.js?
is a progressive framework for building user interfaces. 

   * Vue.js lets you extend HTML with HTML attributes called directives
   * Vue.js directives offers functionality to HTML applications
   * Vue.js provides built-in directives and user defined directives

## Getting Starrted
### The Vue Instance
~~~
var app = new Vue({ options })
~~~
    A Vue instance is the root of our application. It is created by passing an options object into it. Just like it sounds, this object has a variety of optional properties that give the instance the ability to store data and perform actions.

### Plugging in to an Element
~~~
el: '#app'
~~~
    The Vue instance is then plugged into an element of your choosing, forming a relationship between the instance and that portion of the DOM. In other words, we’re activating Vue on the div with the id of app by setting '``#app``' as the element ( el ) that our instance is plugged into.

### Putting our data in its place
A Vue instance has a place for data, in its data property.
~~~
data:{
    element:"value"
}
~~~
The instance’s data can be accessed from inside the element that the instance is plugged into.

### Using an Expression
    If we want our attr to appear in our h1, we can put attr inside these double curly braces.
~~~
<h1> {{ attr }}
~~~
**Important Term: Expression**
Expressions allow us to utilize existing data values, together with logic, to produce new data values.
**Some other ways expressions can be used:**
~~~
{{ product + '?'}}
{{ firstName + ' ' + lastName}}
{{ message.split(' ').reverse().join(' ')}}
~~~
### introducing Reactivity
    The reason Vue is able to display element ‘s value immediately is because Vue is reactive. In other words, the instance’s data is linked to every place that data is being referenced. So not only can Vue make its data appear within the HTML that references it, but that HTML will be updated to display new values any time that referenced data changes.
## Abb
* The Vue instance is the root of every Vue application
* The Vue instance plugs into an element in the DOM
* The Vue instance’s data can be displayed using the mustache-like syntax {{ }} called an expression.
* Vue is reactive
