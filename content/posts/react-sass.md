# What is Sass
**Sass** is a **CSS** pre-processor.
**Sass** files are executed on the server and sends **CSS** to the browser.
more about Sass in [Sass docs](https://sass-lang.com/documentation).
## Quick Start
1. installing SASS in react-app
~~~
npm install node-sass
~~~
2. Change .css files to .scss
3. Change any imports to use .scss
## Using and Sharing Sass Variables
We can import our Sass files from other Sass files and use it
**Example:**
**Create a Sass file:**
    Create a Sass file the same way as you create CSS files, but Sass files have the file extension .scss
    In Sass files you can use variables and other Sass functions:
~~~
$myColor: red;

h1 {
  color: $myColor;
}
~~~