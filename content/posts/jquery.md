+++
title = "JQuery"
date = "2019-11-22"
draft = false
pinned = false
image = "/img/jquery.jpg"
+++
## jQuery Syntax
With `JQuery` you select `(query)` HTML elements and perform **"actions"** on them

```js
$(selector).action()
```
This is to prevent any jQuery code from running before the document is finished loading (is ready).
### The Document Ready Event

```js
$(document).ready(function(){
    //
})
```
Here are some examples of actions that can fail if methods are run before the document is fully loaded:

* Trying to hide an element that is not created yet
* Trying to get the size of an image that is not loaded yet
```js
<head>
<script src="https://ajax.aspnetcdn.com/ajax/jQuery/jquery-3.4.1.min.js">
</script>
<script>
$(()=> $("button").click(()=> $("p").hide()))
</script>
</head>

<body>
<h2>Heading</h2>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaer</p>
<button>Click</button>
</body>
```js
Syntax                   | Description
-------------------------|:-----------
$(*)                     |Selects all elements		
$(this)                  |Selects the current HTML element	
$("p.intro")             |Selects all <p> elements with class="intro"	
$("p:first")             |Selects the first <p> element	
$("ul li:first")         |Selects the first <li> el of the first <ul>
$("ul li:first-child")   |Selects the first <li> el of every <ul>	
$("[href]")              |Selects all el with an href attribute
$("a[target="Blank"]")   |Selects all <a> el with a target att value equal to "_blank"
$("a[target!="blank"]")  |Selects all <a> el with a target att value NOT equal to "_blank"
$(":button")             |Selects all <button> el and <input> el of type="button"
$("tr:even")             |Selects all even <tr> el
$("tr:odd")              |Selects all odd <tr> el
```
## JQuery Effects

### hide() and show()
Syntax:
`$(selector).hide/show(speed,callback);`

```js
<head>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    <script>
        $(() => {
            $("#hide").on("click", () => $("p").hide())
            $("#show").on("click", () => $("p").show())
        });
    </script>
</head>

<body>
    <p>Show / Disappear</p>
    <button id="hide">Hide</button>
    <button id="show">Show</button>
</body>

```
### toggle()
to toggle between **hiding** and **showing** an element with the `toggle()` method

[toggle burger Menu](https://github.com/chiarabdy/lernblog/blob/master/content/challenges/js/toggle.html)

