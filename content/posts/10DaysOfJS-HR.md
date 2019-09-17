+++
title = "10 Days of JS"
date = "2019-09-06"
draft = false
pinned = true
image = "/img/hackerrank.png"
+++
# Overview: 10 Days of JavaScript

    This series focuses on learning and practicing JavaScript. Each challenge comes with a tutorial article, and you 
    can view these articles by clicking either the Topics tab along the top or the article icon in the right-hand menu.
## Day 0: Hello, World!
A greeting function is provided for you in the editor below. It has one parameter, . Perform the following tasks to complete this challenge:
### Task
1. Use console.log() to print Hello, World! on a new line in the console, which is also known as stdout or standard output. The code for this portion of the task is already provided in the editor.
2. Use console.log() to print the contents of (i.e., the argument passed to main).

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day00/helloWorld.js)

## Day 0: Data Types
### Task
Variables named **firstInteger**, **firstDecimal**, and **firstString** are declared for you in the editor below. You must use the **+**  operator to perform the following sequence of operations:

1. Convert **secondInteger** to an integer (Number type), then sum it with **firstInteger** and print the result on a new line using console.log.
2. Convert **seconDecimal** to an floating-point number (Number type), then sum it with **firstDecimal** and print the result on a new line using console.log.
3. Print the concatenation of **firstString** and **secondString** on a new line using console.log. Note that **firstSring**  must be printed first.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day00/dataTypes.js)

## Day 01: Arithmetic Operators
### Task
Complete the following functions in the editor below:
1. getArea(length, width): Calculate and return the area of a rectangle having sides **length** and **width** .
2. getPerimeter(length, width): Calculate and return the perimeter of a rectangle having sides **length** and **width** .
The values returned by these functions are printed to stdout by locked stub code in the editor.
### Explanation 0
* The area of the rectangle is **length** x **width** = 4 x 4.5 = 13.5 .
* The perimeter of the rectangle is 2.(**length** + **width**) = 2.(3 + 4.5) = 15.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day01/arithmetic.js)
## Day 01: Functions
### Task
Implement a function named factorial that has one parameter: an integer,**n** . It must return the value of **n**! (i.e., n factorial).
**Problem**
* A integer of value n is provided
* 1 ≤ n ≤ 10
* Output the factorial value of n (n!, 4! = 4 x 3 x 2 x 1 = 24)

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day01/Functions.js)

## Day 01: Let and Const
### Task
* Declare a constant variable,**PI** , and assign it the value Math.PI. You will not pass this challenge unless the variable is declared as a constant and named PI (uppercase).
* Read a number,**r** , denoting the radius of a circle from stdin.
* Use **PI** and **r** to calculate the **area** and **perimeter** of a circle having radius .
* Print **area** as the first line of output and print **perimeter** as the second line of output.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day01/letAndConst.js)

## Day 2: Conditional Statements: If-Else
### Task
Complete the getGrade(score) function in the editor. It has one parameter: an integer,**score** , denoting the number of points Julia earned on an exam. It must return the letter corresponding to her **grade** according to the following rules:

    If 25 < score <= 30, then grade = A.
    If 20 < score <= 25, then grade = B.
    If 15 < score <= 20, then grade = C.
    If 10 < score <= 15, then grade = D.
    If 5 < score <= 10, then grade = E.
    If 0 <= score <= 5, then grade = F.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day02/%C2%96If-Else-Statements.js)

## Day 2: Conditional Statements: Switch
### Task:
Complete the getLetter(s) function in the editor. It has one parameter: a string, **s**, consisting of lowercase English alphabetic letters (i.e., a through z). It must return A, B, C, or D depending on the following criteria:

If the first character in string **s** is in the set {a ,e ,i ,o ,u } then return A.
If the first character in string **s** is in the set {b,c ,d ,f ,g } then return B.
If the first character in string **s** is in the set {h ,j ,k ,l ,m } then return C.
If the first character in string **s** is in the set {n ,p ,q ,r ,s , t , v, w, x,y, z}, then return D.
Hint: You can get the letter at some index  in  using the syntax s[i] or s.charAt(i).
