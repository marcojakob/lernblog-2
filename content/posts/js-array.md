+++
title = "JavaScript Array"
date = "2019-11-18"
draft = false
pinned = false
image = "/img/array.png"
+++
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
#### Remove an items by index position

```js
const removeItem = Array.splice(pos, index);
```
#### Remove items from an index position

```js
const numbers = ['Zero', 'One', 'Two', 'Three', 'Four'];

const pos = 1, n = 2;

const removeNum = numbers.splice(pos, n); 
console.log(numbers); 
//['Zero', 'One', 'Two', 'Three', 'Four'];

console.log(removedItems); 
// ["Two", "Three"]
```