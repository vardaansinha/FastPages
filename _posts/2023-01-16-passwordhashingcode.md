---
toc: true
layout: post
description: Password Hashing Research in Relation to CPT
categories: [markdown]
title: Password Hashing Research in Relation to CPT
---

When working on the frontend development of the CPT (the login and signup page), I did not implement a specific feature that is seen on many professional sites: password hashing and security. 

<br>
<br>

On most websites, to ensure that user data is safe, they make sure that when an individual creates an account, the password meets a minimum password length and complexity check (special characters, capital letters, numbers). I really thought that this would be useful and pretty cool to implement on my group's CPT, especially with the relevance that cybersecurity has in our world today. 

**Research** (source: https://web.dev/sign-in-form-best-practices/)

From research, one of the main things I found to combat this issue is to use the "type" attribute. Using the attribute, the code can identify which inputs for a username OR password have invalid characters or do not meet specific requirements.

Therefore, using this feature, our site can make a specific password invalid if it were to not have enough characters or not enough complexity (by our own standards). This is definitely something that we will look to work on.

Furthermore, using the example from the OOP Hacks from the APCSP site, there is a way to encode passwords so that they are not readable in plain text. SHA256, which was used in the example, is not nearly the most secure hashing type, so we will do some more research to see which encryption method is the best to be utilized and we will use that. 