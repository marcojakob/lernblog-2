+++
title = "Array Methods"
date = "2019-11-19"
draft = false
pinned = false
image = "/img/array-methods.png"
+++

## Array.filter()
**Syntax**:
```js
var newArray = arr.filter(callback(element[, index[, array]])[, thisArg])
```
***filter()*** calls a provided ``callback function`` once __for each element in an array__, and constructs a __new array__ of all the values for which callback returns a value that coerces to ```true```.

```js
const companies = [
  { name: "company1", category: "Counting", start: 1988, end: 2018 },
  { name: "company2", category: "Counting", start: 1988, end: 2018 },
  { name: "company3", category: "Counting", start: 1988, end: 2019 },
  { name: "company4", category: "Counting", start: 1988, end: 2019 },
  { name: "company5", category: "Counting", start: 1988, end: 2020 },
  { name: "company6", category: "Counting", start: 1988, end: 2020 },
  { name: "company7", category: "Counting", start: 1988, end: 2021 },
  { name: "company8", category: "Counting", start: 1988, end: 2021 },
  { name: "company9", category: "Counting", start: 1988, end: 2022 }
]
//filter()
const filteredItems = companies.filter((company) => {
  return company.end === 2018;
})
console.log(filteredItems)
```

## Array.map()
**Syntax**
```js
const new_array = arr.map(function callback(currentValue[, index[, array]]) {
    // Return element for new_array
}[, thisArg])
```
The __map()__ method creates a ``new array`` with the results of calling a provided function on every element in the calling array
```js
//map()
const itemsName = companies.map((company)=>{
  return item.name
})
console.log(itemsName)
```
#### Using map to reformat objects in an array

```js
const kvArray = [
  { key: 1, value: 10, value02: 1 },
  { key: 2, value: 20, value02: 10 },
  { key: 3, value: 30, value02: 100 }
];

const reformattedArray = kvArray.map((item, index, Array) => {
  // console.log(kvArray.value)
  // var rObj = {};
  let rObj = new Object()
  rObj[item.key] = item.value02
  //console.log
  return rObj
});
console.log(reformattedArray)
```

## Array.find()
```js
const findCompany = companies.find((company)=>{
  return company.name == 'company6';
})
console.log(findCompany)
//{ name: "company6", category: "Counting", start: 1988, end: 2020 }
```

## Array.reduce()
**Syntax**:
```js
arr.reduce(callback(accumulator, currentValue[, index[, array]])[, initialValue])
```
The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.
```js
let vals = [1,2,3,5,6,7,9]
  // let acc = 0;
  // for(val of vlas){
  //   acc += vla ;
  // }
  // console.log(acc)
  //
let reduceVal = vals.reduce((acc, val) => acc + val);
console.log(reduceVal);
```