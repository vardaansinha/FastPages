# Binary Math
Learn some cool stuff about binary math!


## What Are Binary Numbers?

Binary numbers are numbers that are expressed using the base 2 number system, rather than the base 10 decimal system that we are all used to (1,2,3,4,5,etc). Additionally, with binary, there are only two possible values, 0 and 1, with 0 indicating that it is false or "off" and 1 indicating that it is true or "on" (more about that later on). No in betweens!


## What Do We Use Binary Numbers For?

It seems strange to use a base 2 number system that only consists of 0s and 1s; however, binary numbers have uses for a lot more things than you would probably expect. For example, binary allows devices to store, access, and manipulate all sorts of data directed to and from the CPU or memory. This allows us to perform some of the stuff that we like to do on our computers every day, such as viewing websites, playing games, creating and updating documents, and so much more. While we may not use the binary number system at our school (and probably in most schools around the world), binary numbers play a major role when it comes to the world of computer science. Machine language, which is language understood by the computer, is made up of all binary numbers
- Machine language usually displayed in hexadecimal form so that it is easier to read
- Programming languages provide connection between human thought processes and the binary works of machine language that control computer actions

## Conversion

Apart from their uses in our computers, we can also convert that series of 0s and 1s to the original decimal numbers that we are all familiar with.


### How Do We Convert Decimal Numbers to Binary Numbers? (Sample Code)

```
def convertToBinary(n):
    # b represents the binary number
    b = ""

    # n represents the decimal number that will be converted into the binary number
    while n > 0:
    
    # r represents the remainder
        r = n % 2
        b = str(r) + b
        n = n // 2
    return b.zfill(8)

n = int(input("What decimal number would you like to convert to binary?"))
print("User input: ", n)
b = convertToBinary(n)
print("The number {} in binary is {}".format(n,b))

```

Output would look something like this:

```

What decimal number would you like to convert to binary?83
User input:  83
The number 83 in binary is 01010011

```

In English terms, we can convert decimal numbers to binary numbers by repeatedly dividing the decimal number inputted until its quotient is zero. We then reverse the order of the remainders in order to get that decimal number in binary. Here is what the process would like if you were to do this yourself, using the number 106 as an example:

| Decimal Number | Quotient | Remainder |
|------------------|----------|-----------|
| 106 | N/A | N/A |
| 106/2 | 53 | 0 |
| 53/2 | 26 | 1 |
| 26/2 | 13 | 0 |
| 13/2 | 6 | 1 |
| 6/2 | 3 | 0 |
| 3/2 | 1 | 1 |
| 1/2 | 0 | 1 |

| Decimal Number | Decimal Number in Binary |
|----------------|--------------------------|
| 106 | 1101010 |


You may have noticed that we ended up having to reverse the order the remainders appeared in order to get the number 106 into binary. This is done due to the concepts of the least significant bit (LSB) and the most significant bit (MSB). The LSB corresponds to the rightmost digit of the binary number while the MSB corresponds to the leftmost digit. Therefore, in order to get the correct order of 0s and 1s, we need to reverse the order of the remainders. 


### How Do We Convert Binary Numbers to Decimal Numbers? (Sample Code)

```

def convertToDecimal(b):
    # n represents the decimal number
    n = 0
    
    # p represents the position (power) of the binary digit (2 raised to the 0, to the 1st, to the 2nd, etc.)
    p = 0
    
    # goes through the binary digits from right to left
    for digit in reversed(b):
        if digit == '1':
            n += 2 ** p
        p += 1
    
    return n

b = input("What binary number would you like to convert to decimal? ")
print("User input: ", b)
n = convertToDecimal(b)
print("The number {} in decimal is {}".format(b, n))

```

Output would look something like this:

```

What binary number would you like to convert to decimal? 10101010
User input:  10101010
The number 10101010 in decimal is 170

```
In English, we can convert binary numbers back to their decimal numbers by using each bit's corresponding position and power of 2. For example, in converting 10101010 to decimal, for the rightmost '1', we would have 2 raised to the power of 1 and therefore add it to any decimal number that we obtain from doing this. Once we have done this for all of the 1s, we add up all the numbers we get from raising 2 to whichever power to get our decimal number. Below is an illustration of what this would look like if you were to do it yourself, using 11001010 as an example:

|---|---|---|---|---|---|---|---|---|
| **Binary Digit** | 1 | 1 | 0 | 0 | 1 | 0 | 1 | 0 |
| **Power of 2** | 2^7 | 2^6 | 0 | 0 | 2^3 | 0 | 2^1 | 0 |
| **Decimal Number** | 128 | 64 | 0 | 0 | 8 | 0 | 2 | 0 |

```
128+64+8+2 = 202
Therefore, 11001010 in decimal is 202.

```

### Conversion Exercises 

Convert the following numbers to decimal notation:
The binary number 111.
The binary number 1011.
The binary number 10111011.

## Interactions With Binary Math

While converting decimal numbers to binary numbers and vice versa is an important use of binary math, binary numbers also allow us to create interesting interactions for the user to play around with. For example, out on the Internet, there are several binary calculators available to everyone. They allow you to add, subtract, multiply, and divide binary numbers!


Play around with the buttons below, which allow you to input two binary numbers and provides you with the output of the sum. Write down any notes/observations about this and see if you can get an idea of how we can add binary numbers together (required). Try to make your best guess before moving on!

{% include binarymath.html %}

There are actually rules that need to be followed when it comes to adding up binary numbers. Below is a table displaying these rules. 


**Adding Binary Numbers Rules**

|---------|---|
| **1+1** | 0 (carry a 1) |
| **1+0** | 1 | 
| **0+1** | 1 | 
| **0+0** | 0 |



- Machine language refers to the language understood by the computer

- Machine language made up of instructions that are all binary numbers
- Machine language usually displayed in hexadecimal form so that it is easier to read
- Programming languages provide connection between human thought processes and the binary works of machine language that control computer actions

## Overflow/Rounding Errors

### Overflow Errors

Overflow errors result from when we add two binary numbers together, with each binary holding a certain number of bits, but the answer ends up having more bits than the binary can actually stores, thus causing an overflow error and sometimes yielding the wrong result.

The diagram below is a perfect example of overflow errors and how they work:

![]({{site.baseurl}}/images/overflow.png)

### Roundoff Errors

Roundoff or rounding errors in binary results from the inability of the computer to precisely represent some numbers.  Below is another representation of rounding errors and how they work: 

![]({{site.baseurl}}/images/roundoff.png)


## Abstraction of Data Using Binary

You are probably familiar with data abstraction by now, as that is one of the main things that we have discussed and learned about this year. It also happens to be one of the rows on College Board's Rubric for the Create Performance Task. If you happen to forget what data abstraction was, below is a description of the data abstraction row on the rubric: 

![]({{site.baseurl}}/images/dataabstraction.png)

Relating binary and data abstraction together, binary sequences (consisting of values that can either be 0s or 1s, of course) can be used to represent more complex sets of data that we encounter in our day to day lives. In fact, everything in our computer is represented as a binary sequence. 


## Analog and Digital Representation

Computers only have the ability to store digital data, with the most common example of digital data being binary. This is because while analog data is infinitely detail, computers can only hold finite sets of data in a binary representation.

![]({{site.baseurl}}/images/analogdigital.jpg)



## Hacks


**Question**: How do you think we should find the difference of two binary numbers? The product? The quotient? What rules need to be followed for those operations? Look into all of this on the Internet and note down important information you find (0.45)



Based on what you find online, fill out the tables below for subtracting, multiplying, and dividing binary numbers (0.45):


**Subtracting Binary Numbers Rules**

|---------|---------|---------|---------|
| **1-1** | **1-0** | **0-1** | **0-0** |
|    ?     |     ?    |     ?    |     ?    |


**Multiplying Binary Numbers Rules**


|---------|---------|---------|---------|
| **1x1** | **1x0** | **0x1** | **0x0** |
|    ?     |     ?    |    ?     |    ?     |


**Dividing Binary Numbers Rules**

|---------|---------|
| **1/1** | **0/1** |
|     ?    |    ?    |        


Choose ONE (0.9 for doing one):

- Create buttons similar to the ones above that allow you to **subtract** binary numbers and returns the desired result in both binary and decimal
- Create buttons similar to the ones above that allow you to **multiply**  binary numbers and returns the desired result in both binary and decimal
- Create buttons similar to the ones above that allow you to **divide**  binary numbers and returns the desired result in both binary and decimal

If you create buttons for all three of these (or somehow find a way to combine them!), you can get an extra 0.1, and if you decide to customize the buttons to make them look more visually appealing (i.e. by using SASS), you could get extra credit.


**BONUS**: Create a binary to decimal/decimal to binary converter in any language (not given in the lesson) a different way (0.9). Try not to use binary functions (like bin(x))!





