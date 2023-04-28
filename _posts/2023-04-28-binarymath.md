---
toc: true
layout: post
description: Binary Math Hacks
categories: [markdown]
title: Binary Math Hacks
---
### Conversion Exercises 

Convert the following numbers to decimal notation:
The binary number 111.: **7**
The binary number 1011.: **11**
The binary number 10111011.: **187**

## BINARY MATH HACKS

DIFFERENCES OF BINARY MATH NUMBERS:

{% include binarymath.html %}


## Hacks


**Question**: How do you think we should find the difference of two binary numbers? The product? The quotient? What rules need to be followed for those operations? Look into all of this on the Internet and note down important information you find (0.45) 

**For subtracting two binary numbers, it is very similar to subtracting base 10 numbers. When 1 is subtracted from 0, it is necessary to borrow 1 from the next highest bit and then the bit is reduced by 1 with a remainder of 1. For multiplying binary numbers, the product is always 0 or the binary number itself. For each non-zero you have to shift the multiplier to the left and then add the shifted numbers together. Finally, for dividing two binary numbers, there are a couple of rules (as filled out below) and you cannot divide by 0 (it yields nothing). If the divisor is greater than the dividend, the 0 is set as the quotient and the second bit of the dividend is brought down, but if the dividend is larger, you multiply the divisor by 1 and the result is subtracted. Then, you find the remainder, perform the first step again, and then keep going until the remainder is 0.**



Based on what you find online, fill out the tables below for subtracting, multiplying, and dividing binary numbers (0.45):


**Subtracting Binary Numbers Rules**

|---------|---------|---------|---------|
| **1-1** | **1-0** | **0-1** | **0-0** |
|    0     |     1    |     1    |     0    |


**Multiplying Binary Numbers Rules**


|---------|---------|---------|---------|
| **1x1** | **1x0** | **0x1** | **0x0** |
|    1     |     0    |    0     |    0     |


**Dividing Binary Numbers Rules**

|---------|---------|
| **1/1** | **0/1** |
|     1    |    0    |        


Choose ONE (0.9 for doing one):

- Create buttons similar to the ones above that allow you to **subtract** binary numbers and returns the desired result in both binary and decimal

In the above button, I was able to create a button that **subtracts** binary numbers and returns that desired result in both binary and decimal.



