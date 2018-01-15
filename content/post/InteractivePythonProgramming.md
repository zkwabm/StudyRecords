---
title: 'Notes for Open Course: Interactive Python Programming'
author: ''
date: '2018-01-14'
slug: notes-for-open-course-interactive-python-programming
categories: []
tags: []
---
# Notes for the open course - Interactive Python Programming

## Week 1 - Expressions

### An easy environment: Codeskulptor
1. Python2 version: http://www.codeskulptor.org
2. Python3 version: http://py3.codeskulptor.org/

### Arithmetic Expressions


```python
# Arithmetic Expressions - numbers, operators, expressions

print(3, -1, 3.14159, -2.8)
```

    3 -1 3.14159 -2.8
    


```python
# numbers - two types, an integer or a decimal number 
# two corresponding data types int() and float()
print(type(3), type(3.14159))
print(type(3.0))
```

    <class 'int'> <class 'float'>
    <class 'float'>
    


```python
# we can convert between data types using int() and float()
# note that int() takes the 'whole' part of a decimal number
# float() applied to integers is boring
print(int(3.14159), int(-2.8))
print(float(3), float(-1))
```

    3 -2
    3.0 -1.0
    


```python
# floating point number have around 15 decimal digits of accuracy 
# pi is 3.1415926535897932384626433832795028841971...
# square root of two is 1.4142135623730950488016887242096980785696...

# approximation of pi, maintains around 15 decimal digits

print(3.1415926535897932384626433832795028841971)

# approximation of square root of two

print(1.4142135623730950488016887242096980785696)
```

    3.141592653589793
    1.4142135623730951
    


```python
# arithmetic operators
# +   plus         addition
# -   minus        subtraction
# *   times        multiplication
# /   divided by   division
# **  power        exponentiation

print (1 + 2, 3 - 4, 5 * 6, 2 ** 5)

# if one operand is a decimal (float), the answer is decimal
print(1.0 / 3, 5.0 / 2.0, -7 / 3.0, 4 / 2.0)

# division in python 2: If both operands are ints, the answer is an int (rounded down)
# in Python 3, the answer is decimal
print (1 / 3, 5 / 2, -7 / 3, 4 / 2)

```

    3 -1 30 32
    0.3333333333333333 2.5 -2.3333333333333335 2.0
    0.3333333333333333 2.5 -2.3333333333333335 2.0
    


```python
# expressions - number or a binary operator applied to two expressions
# minus is also a unary operator and can be applied to a single expression
print (1 + 2 * 3, 4.0 - 5.0 / 6.0, 7 * 8 + 9 * 10)

# expressions are entered as sequence of numbers and operations
# how are the number and operators grouped to form expressions?
# operator precedence - 'please excuse my dear aunt sallie' = (), **, *, /, +, -
print (1 * 2 + 3 * 4)
print(2 + 12)

# always manually group using parentheses when in doubt
print (1 * (2 + 3) * 4)
print (1 * 5 * 4)
```

    7 3.1666666666666665 146
    14
    14
    20
    20
    

### Practice Exercise for Expressions


```python
# 1 Miles to feet
# There are 5280 feet in a mile. Write a Python statement that calculates and prints the number of feet in 13 miles.

# Compute the number of feet corresponding to a number of miles.

###################################################
# Miles to feet conversion formula
# Student should enter statement on the next line.

print (13 * 5280)

###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#68640
```

    68640
    


```python
# 2 Hours to seconds
# Write a Python statement that calculates and prints the number of seconds in 7 hours, 21 minutes and 37 seconds.

# Compute the number of seconds in a given number of hours, minutes, and seconds.

###################################################
# Hours, minutes, and seconds to seconds conversion formula
# Student should enter statement on the next line.

print (7 * 3600 + 21 * 60 + 37)

###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#26497
```

    26497
    


```python
# 3 Perimeter of rectangle
# The perimeter of a rectangle is 2w+2h, where w and h are the lengths of its sides. 
# Write a Python statement that calculates and prints the length in inches of the perimeter of a rectangle with sides of length 4 and 7 inches.

# Compute the length of a rectangle's perimeter, given its width and height.

###################################################
# Rectangle perimeter formula
# Student should enter statement on the next line.

print (2 * 4 + 2 * 7)

###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#22

```

    22
    


```python
# 4 Area of rectangle
# The area of a rectangle is wh, where w and h are the lengths of its sides.
# Note that the multiplication operation is not shown explicitly in this formula. 
# This is standard practice in mathematics, but not in programming. 
# Write a Python statement that calculates and prints the area in square inches of a rectangle with sides of length 4 and 7 inches.

# Compute the area of a rectangle, given its width and height.

###################################################
# Rectangle area formula
# Student should enter statement on the next line.

print (4 * 7)
###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#28
```

    28
    


```python
# 5 Circumference of circle
# The circumference of a circle is 2πr where r is the radius of the circle. 
# Write a Python statement that calculates and prints the circumference in inches of a circle whose radius is 8 inches. 
# Assume that the constant π=3.14.

# Compute the circumference of a circle, given the length of its radius.

###################################################
# Circle circumference formula
# Student should enter statement on the next line.

print (2 * 3.14 * 8)

###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#50.24
```

    50.24
    


```python
# 6 Area of circle
# The area of a circle is πr2 where r is the radius of the circle. (The raised 2 in the formula is an exponent.) 
# Write a Python statement that calculates and prints the area in square inches of a circle whose radius is 8 inches. 
# Assume that the constant π=3.14.

# Compute the area of a circle, given the length of its radius.

###################################################
# Circle area formula
# Student should enter statement on the next line.

print (3.14 * (8 ** 2))
###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#200.96

```

    200.96
    


```python
# 7 Future Value
# Given p dollars, the future value of this money when compounded yearly at a rate of r percent interest for y years is p(1+0.01r)^y.
# Write a Python statement that calculates and prints the value of 1000 dollars compounded at 7 percent interest for 10 years.

# Compute the future value of a given present value, annual rate, and number of years.

###################################################
# Future value formula
# Student should enter statement on the next line.

print (1000 * (1 + 0.01 * 7) ** 10)

###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#1967.15135729
```

    1967.1513572895665
    


```python
# 8 Name tag
# Write a single Python statement that combines the three strings "My name is", "Joe" and "Warren" (plus a couple of other small strings) into one larger string "My name is Joe Warren." and prints the result.

# Compute a name tag, given the first and last name.

###################################################
# Name tag formula
# Student should enter statement on the next line.

print ("My name is " + "Joe " + "Warren" + ".")
###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#My name is Joe Warren.
```

    My name is Joe Warren.
    


```python
# 9 Name and age
# Write a Python expression that combines the string "Joe Warren is 52 years old.
# " from the string "Joe Warren" and the number 52 and then prints the result 
# (Hint: Use the function str to convert the number into a string.)

# Compute the statement about a person's name and age, given the person's name and age.

###################################################
# Name and age formula
# Student should enter statement on the next line.
print ("Joe Warren" + " is " + str(52) + " years old.")


###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#Joe Warren is 52 years old.


```

    Joe Warren is 52 years old.
    


```python
# 10 The distance between two points (x0,y0)
# (x0,y0) and (x1,y1) is √(x0−x1)2+(y0−y1)^2. 
# Write a Python statement that calculates and prints the distance between the points (2,2) and (5,6).

# Compute the distance between the points (x0, y0) and (x1, y1).

###################################################
# Distance formula
# Student should enter statement on the next line.

# Hint: You need to use the power operation ** .

print (((6 - 2) ** 2 + (5 - 2) ** 2) ** 0.5) 

###################################################
# Expected output
# Student should look at the following comments and compare to printed output.

#5.0
```

    5.0
    


```python

```
