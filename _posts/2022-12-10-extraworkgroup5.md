---
toc: true
layout: post
description: Extra Research Sections 9-11
categories: [markdown]
title: Extra Research Sections 9-11
---

Based on some additional research on the binary searching algorithm, I found out that this method is used in many other different programming languages as well, not JUST Python.

Through this research, I looked at how binary searching is done in C. 

For some context, C and Python have a few differences:

- C is *statistically typed*, while Python is *dynamically typed*. The difference between the two is that statistically typed languages do NOT check types during code execution (is established before running a program), which allows for better runtime performance.
- C does *not* have complex data structures like Python does.
- Testing and debugging in C is slightly harder than it is in Python.

**Analysis**:

![]({{site.baseurl}}/images/extrastuffbinary.png "An example of a binary searching program in C.")

In this program, the most important line is seen in line **4**. It says, "int i, low, high, mid, n, key, array[100];". 

Breaking this down, we can see that there is a clear array of values being set. the "i" is used to iterate through that array. Then, drawing some similarities to the lesson about binary searching, we see that there is, low, high, and middle. The "low" value includes the *first* array index value, the "high" value includes the *high* array index value, and the middle is the *middle index value*, which we have experience in calculating (high + low all divided by 2). Then, we see that there is an "n". This is the number of elements that are in the set array. Finally, "key" is the element that is being searched.

Furthermore, there is some utilization of previous concepts that we have learned in AP CSP. First of all, we see that this program has utilized different types of loops to achieve the final result.

First of all, we see a **for loop** being used. This for loop is needed in order to store the number of elements in the array into the defined variable 'n', and the elements are received by the program from the user. 

Second of all, we also see a **while loop** being used. This loop checks if the lowest array index value is less than the highest array index value (as defined in line 4). This while loop also checks that the middle array index value is less than the key value. 

If the key is greater than the middle array index value, the middle value has one added to it. Then, we keep going until the value is printed and the loop is exited. 

Now, drawing *another* similarity to our hacks from sections 9-11, we see that it is necessary to **sort** the array beforehand. To perform a binary search in C, this array of values that the user inputs must be sorted, otherwise the binary search cannot be performed. 


**TAKEAWAY**:

Each coding language has its separate workarounds, but there are many concepts, such as the binary search, iterations, and other basic programming concepts which overlap.

Each language can help us to better learn another language and broaden our knowledge.