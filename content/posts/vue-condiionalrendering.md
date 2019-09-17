+++
title = "Conditional Rendering"
date = "2019-09-17"
draft = false
pinned = false
image = "/img/c-rendering.jpg"
+++
# Conditional Rendering in Vue
## v-if
The directive v-if is used to conditionally render a block. The block will only be rendered if the directive’s expression returns a truthy value.
~~~
<h1 v-if="awesome">Vue is awesome!</h1>

~~~
It is also possible to add an “else block” with v-else:
~~~
<h1 v-if="awesome">Vue is awesome!</h1>
<h1 v-else>Oh no 😢</h1>
~~~
### v-if in a conditional toggle
Because v-if is a directive, it has to be attached to a single element. But what if we want to toggle more than one element? In this case we can use v-if on a <template> element, which serves as an invisible wrapper. The final rendered result will not include the <template> element.

~~~
<template v-if="ok">
  <h1>Title</h1>
  <p>Paragraph 1</p>
  <p>Paragraph 2</p>
</template>
~~~
## v-else
You can use the v-else directive to indicate an “else block” for v-if:
~~~
<div v-if="Math.random() > 0.5">
  Now you see me
</div>
<div v-else>
  Now you don't
</div>
~~~
    A v-else element must immediately follow a v-if or a v-else-if element - otherwise it will not be recognized.

## v-else-if
The v-else-if, as the name suggests, serves as an “else if block” for v-if. It can also be chained multiple times:
~~~

<div v-if="type === 'A'">
  A
</div>
<div v-else-if="type === 'B'">
  B
</div>
<div v-else-if="type === 'C'">
  C
</div>
<div v-else>
  Not A/B/C
</div>
~~~
## v-show
Another option for conditionally displaying an element is the v-show directive. The usage is largely the same:
~~~
<h1 v-show="ok">Hello!</h1>
~~~
