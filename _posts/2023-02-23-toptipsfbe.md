---
toc: true
layout: post
description: Top Tips for Frontend/Backend Connection Management
categories: [markdown]
title: Top Tips for Frontend/Backend Connection Management
---



**TOP TIPS FOR MANAGING YOUR FRONTEND/BACKEND CONNECTION**:


1. It is much easier to use POSTMAN to generate your Fetch code instead of trying to write it yourself. Even if it may not contain everything you need, it provides the basic framework you need to include in your frontend code to fetch from your backend. To do so, you have to **create a request**, and then click the **code icon** on the right. Change the dropdown bar to "JavaScript Fetch", and you should be good to go. Below is an example of what it should look like:

![]({{site.baseurl}}/images/fetch.png "What the fetch code looks like from POSTMAN")

2. Make sure you are putting your fetch code in the right place. This involves a little bit of intuition, as you have to realize that the "fetch" is for fetching the data from your backend to put on your frontend so that it is visible for a consumer. Therefore, in whichever file you are focusing on for the frontend in your feature, that is where the fetch code will go. Remember to put this inside of a script tag, as this is JS code in a markdown/HTML file.

3. Make sure you have error conditions to combat any sort of invalid inputs and corrupted fetches from your backend. This will be located in your API/MODEL files, where you can set certain conditions based on what a user inputs, and try to filter out any sort of garbage data from your site. Here is an example of what an error condition can look like: 

![]({{site.baseurl}}/images/error.png "A sample error code which you can put so that your frontend is not inputting garbage data into your backend DB")

