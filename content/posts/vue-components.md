+++
title = "Vue Components"
date = "2019-09-23"
draft = false
pinned = false
description = ""
image = "/img/vue-getting-started.jpg"
+++
## Introduction to Components
Components are reusable Vue instances with a name: in this case, <button-counter>. We can use this component as a custom element inside a root Vue instance created with new Vue:
### compontnt syntax in vue
~~~
Vue.component('name', {}
~~~
**Example**
~~~
Vue.component('button-counter', {
  data: function () {
    return {
      count: 0
    }
  },
  template: '<button v-on:click="count++">You clicked me {{ count }} times.</button>'
})
~~~