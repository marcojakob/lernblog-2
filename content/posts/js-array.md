+++
title = "JavaScript Array"
date = "2019-11-18"
draft = false
pinned = false
image = "/img/array.png"
+++
## Static methods
* Array.from()
Creates a new Array instance from an array-like or iterable object.
```js
const list = document.getElementById('root li');
// if we want to iterate through the html list elements we have to convert it into array to use forEach method
Array.from(list).forEach()
```
* Array.isArray()
Returns ***true*** if a variable is an array, if not ***false***.
* Array.of()
Creates a new Array instance with a variable number of arguments, regardless of number or type of the arguments.

## Common operations
### create an array

```js
const items = [
    {name:'Adele', album: 10 },
    {name: 'LinkenPark', album: 22},
    {name: 'Sia', album: 33},
    {name: 'WestLife', album: 46},
    {name: 'Enriqu', album: 55},
    {name: 'ladyGaga', album: 67}
]
```
#### access (index into) an Array item

```js
 items[0]
```
#### Look over an Array

```js
items.forEach(item=>console.log(item))
//syntax: Arr.forEach(function(item, index, array))
```
#### Add to the end of an Array

```js
items.push({name: 'LoreenaMckennitt', album: 100});
```
#### Remove from the end of an Array

```js
items.pop();
//remove ladyGaga from the array 
```
#### Remove from front of an Array

```js
items.shift();
// Remove Adele
```
#### Add into the front of the Array

```js
items.unshift()
```
#### Find the index of an item in the Array

```js
const items = ["one", "two", "Three", "Four"]
items.indexOf("two")
// 1
```
#### Find the index of an Object in the Array

```js
const index = items.findIndex((item)=#### {
    return item.name === "LinkenPark"
})
console.log(index)
```
#### Remove or replace an items by index position

```js
//Syntax Array.splice(Number pos(starting position ), Number Amount(how many items to remove), item to replace or update);
const numbers = ['Zero', 'One', 'Two', 'Three', 'Four'];

const removeNum = numbers.splice(0, 1,); 
console.log(numbers); 
//'One', 'Two', 'Three', 'Four'];

console.log(removedItems); 
// ["Zero"]

```
#### Find index method 

```js
const items = [
    {name:'Adele', album: 10 },
    {name: 'LinkenPark', album: 22},
    {name: 'Sia', album: 33},
    {name: 'WestLife', album: 46},
    {name: 'Enriqu', album: 55},
    {name: 'ladyGaga', album: 67}
]
function findItem(sia){
    return sia.album === 33; 
}
console.log(items[findIndex(findItem))
//to access the object:
console.log(items[items.findIndex(findItem)])

```
#### Sorting and Manipulating Arrays
```js
//Reverse
const numbers = ["One", "Two", "Three", "Four","Five"];
numbers.reverse();
//["Five", "Four", "Three", "Two", "One"]

//Sort it alphabetically 
numbers.sort();
//["Five", "Four", "One", "Three", "Two"]
```
#### nested Loops through the array   
```js
let array = [
    [1, 2, 3, 4, 5, 6, 7],
    [12, 22, 33, 44, 55, 66, 77,2],
    [13, 23, 33, 43, 53, 63, 73]
]

const rows = array.length
for(let i = 0; i < rows; i++){
    let items = array[i].length;
    console.log(i, items)
    
    for(let n = 0;n < items; n++){
     console.log(array[i][n])   
    }
}
```