+++
title = "Python - Data Types"
date = "2019-10-16"
draft = false
pinned = false
image = "/img/python.jpg"

+++
    Python has the following standard or built-in data types:

## Numeric
Python supports **integers**, **floating point numbers** and **complex numbers**. They are defined as ``int``, ``float`` and ``complex`` class in Python.
```py
a = 5

# Output: <class 'int'>
print(type(a))

# Output: <class 'float'>
print(type(5.0))

# Output: (8+3j)
c = 5 + 3j
print(c + 3)

# Output: True
print(isinstance(c, complex))

```
## List
Python List is a collection of Values that contain any types that contain any type(float, int, bool, str, list)
### reate a list
```py
# empty list
my_list = []
# list of integers
my_list = [1, 2, 3]
# list with mixed datatypes
my_list = [1, "Hello", 3.4]
```
__Also, a list can even have another list as an item. This is called nested list.__ <br>
```py
# nested list
my_list = ["mouse", [8, 4, 6], ['a']]
```
### Access elements in the list

```py
my_list = ['p','r','o','b','e']
# Output: p
print(my_list[0])
# Output: o
print(my_list[2])
# Output: e
print(my_list[4])
# Error! Only integer can be used for indexing
# my_list[4.0]
# Nested List
n_list = ["Happy", [2,0,1,5]]
# Nested indexing
# Output: a
print(n_list[0][1])    
# Output: 5
print(n_list[1][3])
```
### Negative indexing

```py
my_list = ['p','r','o','b','e']
# Output: e
print(my_list[-1])
# Output: p
print(my_list[-5])
```
![Python List Indexing](/img/python-list-index.png "Python-list")

### slice lists in Python
```py
my_list = ['p','r','o','g','r','a','m','i','z']
# elements 3rd to 5th
print(my_list[2:5])
# elements beginning to 4th
print(my_list[:-5])
# elements 6th to end
print(my_list[5:])
# elements beginning to end
print(my_list[:])
```
![Element Slicing](/img/element-slicing.jpg "Element-list")

### change or add elements to a list
```py
# mistake values
odd = [2, 4, 6, 8]
# change the 1st item    
odd[0] = 1            
# Output: [1, 4, 6, 8]
print(odd)
# change 2nd to 4th items
odd[1:4] = [3, 5, 7]  
# Output: [1, 3, 5, 7]
print(odd) 
```
We can add one item to a list using append() method or add several items using extend() method.
```py
odd = [1, 3, 5]
odd.append(7)
# Output: [1, 3, 5, 7]
print(odd)
odd.extend([9, 11, 13])
# Output: [1, 3, 5, 7, 9, 11, 13]
print(odd)
```
We can also use + operator to combine two lists. This is also called concatenation.

```py
odd = [1, 3, 5]
# Output: [1, 3, 5, 9, 7, 5]
print(odd + [9, 7, 5])
#Output: ["re", "re", "re"]
print(["re"] * 3)
```
Furthermore, we can insert one item at a desired location by using the method insert() or insert multiple items by squeezing it into an empty slice of a list.
```py
odd = [1, 9]
odd.insert(1,3)
# Output: [1, 3, 9] 
print(odd)
odd[2:2] = [5, 7]
# Output: [1, 3, 5, 7, 9]
print(odd)
```
### delete or remove elements from a list
```py
my_list = ['p','r','o','b','l','e','m']
# delete one item
del my_list[2]
# Output: ['p', 'r', 'b', 'l', 'e', 'm']     
print(my_list)
# delete multiple items
del my_list[1:5]  
# Output: ['p', 'm']
print(my_list)
# delete entire list
del my_list       
# Error: List not defined
print(my_list)
```
We can use remove() method to remove the given item or pop() method to remove an item at the given index.

The pop() method removes and returns the last item if index is not provided. This helps us implement lists as stacks (first in, last out data structure).

We can also use the clear() method to empty a list.
```py
my_list = ['p','r','o','b','l','e','m']
my_list.remove('p')
# Output: ['r', 'o', 'b', 'l', 'e', 'm']
print(my_list)
# Output: 'o'
print(my_list.pop(1))
# Output: ['r', 'b', 'l', 'e', 'm']
print(my_list)
# Output: 'm'
print(my_list.pop())
# Output: ['r', 'b', 'l', 'e']
print(my_list)
my_list.clear()
# Output: []
print(my_list)
```
Finally, we can also delete items in a list by assigning an empty list to a slice of elements.
```py
>>> my_list = ['p','r','o','b','l','e','m']
>>> my_list[2:3] = []
>>> my_list
['p', 'r', 'b', 'l', 'e', 'm']
>>> my_list[2:5] = []
>>> my_list
['p', 'r', 'm']
```

[Python List Methods](https://www.programiz.com/python-programming/methods/list)

Method             | Description
-------------------|:-----------
append() -         | Add an element to the end of the list
extend() -         | Add all elements of a list to the another list
insert() -         | Insert an item at the defined index
remove() -         | Removes an item from the list
pop() -            | Removes and returns an element at the given index
clear() -          | Removes all items from the list
index() -          | Returns the index of the first matched item
count() -          | Returns the count of number of items passed as an argument
sort() -           | Sort items in a list in ascending order
reverse() -        | Reverse the order of items in the list
copy() -           | Returns a shallow copy of the list
cleasr() -	       | Removes all Items from the List
any()	           | Checks if any Element of an Iterable is True
all()	           | returns true when all elements in iterable is true
ascii()	           | Returns String Containing Printable Representation
bool()	           | Converts a Value to Boolean
enumerate()	       | Returns an Enumerate Object
filter()	       | constructs iterator from elements which are true
iter()	           | returns iterator for an object
list()             | Function	creates list in Python
len()	           | Returns Length of an Object
max()	           | returns largest element
min()	           | returns smallest element
map()	           | Applies Function and Returns a List
reversed()	       | returns reversed iterator of a sequence
slice()	           | creates a slice object specified by range()
sorted()	       | returns sorted list from a given iterable
sum()	           | Add items of an Iterable
zip()	           | Returns an Iterator of Tuple

```py
my_list = [3, 8, 1, 6, 0, 8, 4]
# Output: 1
print(my_list.index(8))
# Output: 2
print(my_list.count(8))
my_list.sort()
# Output: [0, 1, 3, 4, 6, 8, 8]
print(my_list)
my_list.reverse()
# Output: [8, 8, 6, 4, 3, 1, 0]
print(my_list)
```
### Iterating Through a List
Using a for loop we can iterate though each item in a list.


```py
for fruit in ['apple','banana','mango']:
    print("I like",fruit)
```
## String
## Tuple
## Set
## Dictionary

