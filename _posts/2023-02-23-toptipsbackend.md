---
toc: true
layout: post
description: Top Tips for Backend Management
categories: [markdown]
title: Top Tips for Backend Management
---



**TOP TIPS FOR MANAGING YOUR BACKEND**:


1. Make sure that your main file (main.py or app.py, whatever you have it named as) is without any errors before you run your backend server for testing. Having even one error for one class will prevent any sort of functionality from your backend server. To avoid these errors from happening, make sure that you are constantly in communication with your team as to when you are committing, and what you are committing. Often times, it is much safer to run your backend server LOCALLY, so that you can debug errors before you update your files on your deployment server (in our case, this was AWS). 

2. In your "model" and "api" files, you will have to import many modules. Often times, though, when you write the lines to import certain modules, you get errors saying that the "module doesn't exist". To avoid this, make sure that you have "pip install *program*" beforehand, and that the module you are trying to import exists. 

3. Remove any unnecessary lines! Many times, we copy paste a certain backend format so that we have a structure of what we want to do, and then change it to adhere to our own feature. Sometimes, though, there are unnecessary lines, such as modules you may not be using for your feature, or certain DB operations which are not supported by your feature, and it is very important to remove these lines. It can confuse you and throw your backend process off, it can cause a lot of errors in the file because of missing lines not calling certain functions/procedures, and it can also confuse any sort of reader who is looking through your code. 

4. COMMENT! Comments are very important and should be implemented thoroughly into all parts of backend. Backend code can become very confusing, which is why it is important that you put comments for each function, procedure, and parameter, so that you are able to easily debug issues if they come up.