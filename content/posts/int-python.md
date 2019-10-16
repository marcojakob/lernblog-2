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

## Exercise 006 Operations with other types
### Instructions

* Calculate the product of savings and growth_multiplier. Store the result in year1.
* What do you think the resulting type will be? Find out by printing out the type of year1.
* Calculate the sum of desc and desc and store the result in a new variable doubledesc.
* Print out doubledesc. Did you expect this?

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E006.py)

## Exercise 007 Type conversion 
Using the + operator to paste together two strings can be very useful in building custom messages.
```py
print("I started with $" + savings + " and now have $" + result + ". Awesome!")
```
This will not work, though, as you cannot simply sum strings and floats.

To fix the error, you'll need to explicitly convert the types of your variables. More specifically, you'll need str(), to convert a value into a string. str(savings), for example, will convert the float savings to a string.

Similar functions such as int(), float() and bool() will help you convert Python values into any type.
### Instructions
* Hit Run Code to run the code. Try to understand the error message.
* Fix the code such that the printout runs without errors; use the function str() to convert the variables to  strings.
* Convert the variable pi_string to a float and store this float as a new variable, pi_float.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E007.py)

## Exercise 08 Create a list
* Create a list, areas, that contains the area of the hallway (hall), kitchen (kit), living room (liv),
  bedroom (bed) and bathroom (bath), in this order. Use the predefined variables.
* Print areas with the print() function.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E008.py)

## List of lists

* Finish the list of lists so that it also contains the bedroom and bathroom data. Make sure you enter these in order!
* Print out house; does this way of structuring your data make more sense?
* Print out the type of house. Are you still dealing with a list?

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E009.py)

## Subset and conquer
* Print out the second element from the areas list (it has the value 11.25).
* Subset and print out the last element of areas, being 9.50. Using a negative index makes sense here!
* Select the number representing the area of the living room (20.0) and print it out.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E010.py)

## Subset and Calculate
* Using a combination of list subsetting and variable assignment, create a new variable, eat_sleep_area, that contains the sum of the area of the kitchen and the area of the bedroom.
* Print the new variable eat_sleep_area.

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E011.py)

## Slicing and dicing
* Use slicing to create a list, downstairs, that contains the first 6 elements of areas.
* Do a similar thing to create a new variable, upstairs, that contains the last 4 elements of areas.
* Print both downstairs and upstairs using print().

[SOLUTIONS](https://github.com/chiarabdy/lernblog/tree/master/content/challenges/python/E012.py)
