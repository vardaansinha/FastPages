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

