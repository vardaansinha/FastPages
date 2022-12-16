---
layout: page
title: Computer Science Notes
categories: [notes]
permalink: /notes/
---

# Key Terms:

## GitHub-Related Terms:

1. **Repository**: The location (for us, on Github) where we modify our fastpages site and collect all of our work for a particular project.

2. **Clone**: "Cloning" a repository means to copy a repository onto your local system for modification.

3. **Commit**: This means to save and commit changes in order for the changes to update on your site.


## VSCode Terms:

1. **Source Control**: This is the tab in VSCode where you stage, commit, and sync changes.

2. **Debug Console**: This is where you can debug and work around any issues in your VSCode files.


# Application of these Terms:

## Cloning a Repository through WSL:

```bash
(base) vardaan@LAPTOP-6CPSDHS5:~$ cd ./vscode # Changing the directory to your VSCode directory, which contains all of your cloned repositories.
(base) vardaan@LAPTOP-6CPSDHS5:~/vscode$ git clone "https://github.com/SamitPoojary/FASTPAGES.git" # Cloning my partner Samit's FastPages so that I can track his changes.
Cloning into 'FASTPAGES'...
remote: Enumerating objects: 722, done.
remote: Counting objects: 100% (613/613), done.
remote: Compressing objects: 100% (329/329), done.
remote: Total 722 (delta 260), reused 479 (delta 191), pack-reused 109
Receiving objects: 100% (722/722), 9.46 MiB | 1.33 MiB/s, done.
Resolving deltas: 100% (260/260), done.
```

## Checking Status & Making Commits through WSL:

```bash
(base) vardaan@LAPTOP-6CPSDHS5:~/vscode$ dir
APCSP  FASTPAGES  FastPages  fastpages # Showing the files that are in the 'vscode' directory.
(base) vardaan@LAPTOP-6CPSDHS5:~/vscode$ cd ./FastPages
(base) vardaan@LAPTOP-6CPSDHS5:~/vscode/FastPages$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .vscode/settings.json
        modified:   _pages/01_about.md
        modified:   _pages/02_notes.md

no changes added to commit (use "git add" and/or "git commit -a") # This command shows the status of the repository (any modified files or changes that have not been committed). 
(base) vardaan@LAPTOP-6CPSDHS5:~/vscode/FastPages$ git commit -a
[master 746b938] committing large changes for bash committing large changes for bash
 3 files changed, 21 insertions(+), 9 deletions(-) # This commits all the changes, and you can use VSCode to sync the changes.
```
# Key Terms Continued (Trimester Cumulative)

1. **Collaboration**: One of the keys when working with a team on code. It is the art of communication that is essential to making functional code.

2. **Flask**: Web Application Framework that is important to develop web applications.

3. **Jinja2**: The Web Template Language that is compatible with Flask and Python.

4. **Bootstrap**: An HTML/CSS template engine that helps to create more aesthetically appealing sites.

5. **Pseudo Code**: This is essentially another term used to describe the comments that are made to describe each line or functionality of code.

6. **JavaScript**: Another programming language that is essential, especially for frontend developers.

7. **Procedural Abstraction**: The practice of promoting reuse instead of continuously coding the same thing again and again.

8. **Agile Methodology**: The use of pair programming, test-driven development, stand-ups, planning sessions, and sprints. This also includes well defined team roles.

9. **AWS**: Amazon Web Services is a tool that allows for the *deployment* of our projects. It is a large part of the backend of our project.

10. **Nginx**: An open source software used for web serving, reverse proxy, caching, load balancing, media streaming, etc.

11. **Certbot**: This is another open source software tool that allows for encrypted certifications for hosted sites.

12. **DNS**: DNS, or Domain Name Services, allows for the assignment of a friendly name to a web server.

13. **API**: Application Programming Interface, it is a way for multiple programs to communicate/call each other.

14. **API URL**: The endpoint to which the API is directed.

15. **API Headers**: The dictionary data structure used to send special messaging to the endpoint.

16. **Document Object Model**: The Document Object Model, or DOM, is the interaction between HTML and JavaScript.

17. **HTTP/HTTPS**: HTTP, or Hyper Text Transfer Protocol, is in charge of the communication between a web server and web browser. HTTPS, on the other hand, is in charge for more **secure** communication between a web server and a web browser.

18. **TCP/IP**: Transmission Control Protocol, Internet Protocol. These messages are divided into small packets and sent between computers on the Internet.

19. **Network Layer**: The wireless and physical layers that move bits across the Internet.

# Unit 2 Vocabulary:

1. **Bits**: A bit is a binary digit. It is the smallest size of data.

2. **Bytes**: Bytes are groups of bits.

3. **Hexadecimal**: Hex is base 16, and is used to show large values with a fewer amount of digits.  

4. **Unsigned Integer**: These are integers that don't have any associated + or -.

5. **Signed Integer**: These are integers with some sort of directionality (+ or -).

6. **Floating Point**: These are decimals.

7. **Boolean**: Boolean is a binary variable; can either be true or false.

8. **ASCII**: This is a format of character encoding for text on the Internet. 

9. **Unicode**: A character encoding standard that assigns a unique number for each character in almost every language.

10. **RGB**: This is used to represent colors on a system display.

11. *Lossy* and *lossless* have not been discussed yet.

# Unit 3 Vocabulary:

1. **Variables**: Any sort of quantity which can be defined or measured.

2. **Data Types**: These are types of data values.

3. **Assignment Operators**: These are operators which assign values to variables.

4. **Lists**: These are data types that have a number of ordered values. 

5. **2D Lists**: This is a 2D data structure which can represent a matrix.

6. **Dictionaries**: These are a method to store data values through a method known as keys and pairs.

7. **Class**: A class contains all the details about a collection of variables and functions.

8. **Algorithms**: Algorithms are processes which can help to solve certain problems through programming.

9. **Sequence**: A sequence is an ordered set.

10. **Selection**: This selects a certain part of a program to execute based on conditional statements.

11. **Iteration**: This is where the same group of code is repeatedly executed.

12. **Expressions**: These are a combination of operators and data values.

13. **Comparison Operators**: This compares the two values and then tells the user whether the condition is met or not. 

14. **Booleans Expressions and Selection/Iteration**: These are a selection of code that allows for expressions to be iterated through or selected to see if a conditional is true/false (boolean).

16. **Truth Tables**: This is a table to determine if a compound statement is true or false.

17. **Characters**: These are singular keys that go into code.

18. **Strings**: These are arrays of characters.

19. **Length**: This is a function that counts the length of a string.

20. **Concatenation**: Concatenation is the combination of two strings.

21. **Upper**: This makes the string uppercase.

22. **Lower**: This makes the string lowercase.

23. **Traversing Strings**: These are strings that are processed one character at a time.

24. **If Statement**: If a certain conditional is met, then the program will execute some block of code.

25. **Elif Statement**: This checks if the above statement is true.

26. **Else Conditionals**: Again, checks if something is true or not.

27. **Nested Selection Statements**: This is where there is one selection within another. Multiple conditions can be tested here.

28. **For Loops**: These are loops to iterate over a sequence.

29. **While Loops**: While a certain conditional is true, a certain block of code is going to continue running.

30. **List Combining Loops**: These are loops that can combine lists.

31. **Procedural Abstraction**: This is when code sections can be generalized by creating parameters. This is useful, as code blocks can be utilized in multiple different program situations. 

32. **Python def procedures**: These are user-defined procedures.

33. **Parameters**: These are placeholders for variables that a function utilizes.

34. **Return Values**: These are the values that a function returns to the caller.

