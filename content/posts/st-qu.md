+++
title = "Stack and Queues in Js"
date = "2019-11-04"
draft = false
pinned = false
image = "/img/st-qu.png"
+++
What is Stack?
A **Stack** is an ***abstract data type*** that serves as a collection of elements, with two principal operations:
* Push, Which adds an el to the collection, and
* pop, which remove the most recently added element that was not yer removed.

The order in whcih elements come **off** a stack gives rise to its alternative name, ***LIFO*** (las in, first out), Additionally, a **Peek** operation may give access to the top without modifying the stack
```js
const stack = []

//push
stack.push('Qamishlo')
stack.push('Efrin')
stack.push('Kobane')

//pop
stack.pop()

//peek
stack[stack.length -1]

```

### Implement stack using  JS Classes:

```js
class Stack {
  constructor() {
    this.storage = []
    this.size = 0
  }
  
  // Inserts the element into the top of the stack
  push(el){
      this.size++
      this.storage[this.size] = el
  }
  // Removes the element from the top of the stack and return that element
  pop() {
    let removed = this.storage[this.size]
    this.size--
    return removed
  }
  
  // Return which element is on top of the stack
  peek() {
    return this.storage[this.size]
  }
  
  // helper method
  isEmpty() {
    return !this.stack.length
  }
}
```
A ***Queue*** is similar to a stack but the primary differrent between them is stocks are ***LIFO*** while Queues are ***FIFO*** .
The Operation that Queues work with are: ***NQ***: adding to the Queue and ***DQ**: removing from the Queue .

```js
const queue = []

//enqueue (push)
queue.push('Qamishlo')
queue.push('Efrin')
queue.push('Kobane')

//dequeue (shift)
queue.shift()

```

### Implement Queue using  JS Classes:
```js
class Queue {
  constructor() {
    this.queue = []
  }
  
  enqueue(element) {
    this.queue.push(element)
  }
  
  dequeue() {
    if (this.isEmpty()) return 'Queue is empty' 
    return this.queue.shift()
  }
  
  peek() {
    if (this.isEmpty()) return 'Queue is empty'
    return this.queue[0]
  }
  
  // helper method
  isEmpty() {
    return !this.queue.length
  }
}
```