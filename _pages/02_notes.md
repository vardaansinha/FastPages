---
layout: page
title: Computer Science Notes
categories: [notes]
permalink: /notes/
---

## Key Terms:

# GitHub-Related Terms:

1. **Repository**: The location (for us, on Github) where we modify our fastpages site and collect all of our work for a particular project.

2. **Clone**: "Cloning" a repository means to copy a repository onto your local system for modification.

3. **Commit**: This means to save and commit changes in order for the changes to update on your site.


# VSCode Terms:

1. **Source Control**: This is the tab in VSCode where you stage, commit, and sync changes.

2. **Debug Console**: This is where you can debug and work around any issues in your VSCode files.


## Application of these Terms:

# Cloning a Repository through WSL:

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

# Checking Status & Making Commits through WSL:

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
