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

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day02/If-Else-Statements.js)

## Day 2: Conditional Statements: Switch
### Task:
Complete the getLetter(s) function in the editor. It has one parameter: a string, **s**, consisting of lowercase English alphabetic letters (i.e., a through z). It must return A, B, C, or D depending on the following criteria:

If the first character in string **s** is in the set {a ,e ,i ,o ,u } then return A.
If the first character in string **s** is in the set {b,c ,d ,f ,g } then return B.
If the first character in string **s** is in the set {h ,j ,k ,l ,m } then return C.
If the first character in string **s** is in the set {n ,p ,q ,r ,s , t , v, w, x,y, z}, then return D.
Hint: You can get the letter at some index  in  using the syntax s[i] or s.charAt(i)

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day02/ conditionalStatementsSwitch.js)

## Day 2: Loops
### Task
    Complete the vowelsAndConsonants function in the editor below. It has one parameter, a string,**s**, consisting of lowercase English alphabetic letters (i.e., a through z). The function must do the following:

1. First, print each vowel in **s** on a new line. The English vowels are a, e, i, o, and u, and each vowel must be printed in the same order as it appeared in **s**.
2. Second, print each consonant (i.e., non-vowel) in **s** on a new line in the same order as it appeared in **s**.
### Explanation
**Observe the following:**
    Each letter is printed on a new line.
    Then the vowels are printed in the same order as they appeared in .
    Then the consonants are printed in the same order as they appeared in .

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day02/loops.js)

## Day 3: Arrays
### Task 
Complete the getSecondLargest function in the editor below. It has one parameter: an array,**nums** , of **n** numbers. The function must find and return the second largest number in **nums**.

### Explanation
Given the array **nums = [2,3,6,6,5] , we see that the largest value in the array is 6 and the second largest value is 5. Thus, we return 5 as our answer.

* Return the second largest number in the array.
* @param {Number[]} nums - An array of numbers.
* @return {Number} The second largest number in the array.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day03/array.js)
## Day 3: Throw
### Task
Complete the isPositive function below. It has one integer parameter, . If the value of  is positive, it must return the string YES. Otherwise, it must throw an Error according to the following rules:

If **a** is 0, throw an Error with **message -Zero Error**.
If **a** is negative, throw an Error with **message - Negative Error**.

* Complete the isPositive function.
* If 'a' is positive, return "YES".
* If 'a' is 0, throw an Error with the message "Zero Error"
* If 'a' is negative, throw an Error with the message "Negative Error"

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day03/throw.js)

## Day 3: 
### Task
Complete the reverseString function; it has one parameter,**s** . You must perform the following actions:

1. Try to reverse string **s** using the split, reverse, and join methods.
2. If an exception is thrown, catch it and print the contents of the exception's **message** on a new line.
3. Print **s** on a new line. If no exception was thrown, then this should be the reversed string; if an exception was thrown, this should be the original string.
### Output Format

You must write two print statements using console.log():

* Print the contents of a caught exception's **message** on a new line. If no exception was thrown, this line should not be printed.
* Print **s** on a new line. If no exception was thrown, then this should be the reversed string; if an exception was thrown, this should be the original string.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day03/try-catch-finally.js)

## Day 4: Create a Rectangle Object
### Task
Complete the function in the editor. It has two parameters:**a**  and **b**. It must return an object modeling a rectangle that has the following properties:

* length: This value is equal to **a**.
* width: This value is equal to **b**.
* perimeter: This value is equal to **2**.(a +b)
* area: This value is equal to **a.b**

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day04/create-rectangle-object.js)

## Day 4: Count Objects
### Task
Complete the function in the editor. It has one parameter: an array,**a** , of objects. Each object in the array has two integer properties denoted by **x** and **y**. The function must return a count of all such objects **o** in array **a** that satisfy **o.x==o.y** .

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day04/count-objects.js)

## Day 4: Classes
### Task

Create a Polygon class that has the following properties:

* A constructor that takes an array of integer values describing the lengths of the polygon's sides.
* A perimeter() method that returns the polygon's perimeter.
Locked code in the editor tests the Polygon constructor and the perimeter method.

__Note:__ The perimeter method must be lowercase and spelled correctly.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day04/classes.js)

## Day 5: Inheritance
### Task

* Add an area method to Rectangle's prototype.
* Create a Square class that satisfies the following:
    1. It is a subclass of Rectangle.
    2. It contains a constructor and no other methods.
    3. It can use the Rectangle class' area method to print the         area of a Square object.

[SOLUTIONS](https://github.com/chiarabdy/10DaysOfJavaScript-HackerRank/blob/master/day05/inheritance.js)