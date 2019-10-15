+++
title = " introduction to Python for Data Science"
date = "2019-10-15"
draft = false
pinned = false
image = "/img/python.jpg"
+++
# Python Basics
## Exercise 000
### Instructions
* Experiment in the IPython Shell; type 5 / 8, for example.
* Add another line of code to the Python script on the top-right (not in the Shell): print(7 + 10).
* Hit Submit Answer to execute the Python script and receive feedback.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E000.py)

## Python as a calculator
Python is perfectly suited to do basic calculations. Apart from addition, subtraction, multiplication and division, there is also support for more advanced operations such as:
* Exponentiation:`` ** ``. This operator raises the number to its left to the power of the number to its right. For example ``4**2`` will give ``16``.
* Modulo: ``%``. This operator returns the remainder of the division of the number to the left by the number on its right. For example ``18 % 7`` equals ``4``.
## Exercise 001
### instructions
Suppose you have $100, which you can invest with a 10% return each year. After one year, it's 100×1.1=110 dollars, and after two years it's 100×1.1×1.1=121. Add code to calculate how much money you end up with after 7 years, and print the result.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E001.py)

## Exercise 002 Variable Assignment
### Instructions
* Create a variable savings with the value 100.
* Check out this variable by typing print(savings) in the script.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E002.py)

## Exercise 003 Calculations with variables
### Instructions
* Create a variable growth_multiplier, equal to 1.1.
* Create a variable, result, equal to the amount of money you saved after 7 years.
* Print out the value of result.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E003.py)

## Exercise 004 Other variable types
### Instructions
* Create a new string, desc, with the value "compound interest".
* Create a new boolean, profitable, with the value True.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E004.py)

## Exercise 005 Guess the type
To find out the type of a value or a variable that refers to that value, you can use the ```type()``` function. Suppose you've defined a variable a, but you forgot the type of this variable. To determine the type of a, simply execute:

```python
type(a)
```
### Instructions
    choose the correct answer:
* a is of type int, b is of type str, c is of type bool
* a is of type float, b is of type bool, c is of type str
* a is of type float, b is of type str, c is of type bool
* a is of type int, b is of type bool, c is of type str

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E005.py)

