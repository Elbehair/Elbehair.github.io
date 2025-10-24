---
layout: default
---
# Command-Line Course

Welcome to my **Command-Line Tools** course summary!  

This page highlights what I learned in each module — from basic Unix commands to building and deploying a website with Jekyll and GitHub Pages.  

I gained efficiency in the command-line by learning an extensive suite of tools for tasks like scripting, managing software, and processing text.

---

## Module 1: Navigating the Command Line  

I developed fundamental command-line proficiency by exploring basic commands and learning to work with terminal-based text editors.  

We focused on file and directory management, including:  

 * **Manipulating directories**: Learning commands to copy, move, and remove (delete) files and directories.  

 * **Understanding system structure**: Identifying the standard UNIX system directories and what they contain.

 * **Controlling access and privacy**: Understanding how permissions work in UNIX to protect user data and determine which files and directories each user can access.  

The following code is an example if we want to get from the 51st to the 55th line from an input file: 

```bash
head -n 55 numbers_en.txt | tail -n 5
```

I've gained confidence and comfort working within the terminal environment, mastering key navigation skills, including moving between and creating directories. This solid foundation in the command-line has me fully prepared for the next module.  

---

## Module 2: Text Processing in UNIX

We mastered essential UNIX text processing skills to efficiently manage and analyze text data.  

 * We started with the fundamentals of character encodings (how computers read text as binary) and learnt to convert between different formats.

 * We focused on powerful commands for processing and searching text files, which are critical for uncovering patterns in data.

 * We gained proficiency in handling structured text data and, most importantly, learning to combine simple commands into complex pipelines to execute sophisticated operations efficiently.  

A major emphasis was placed on two indispensable tools: the `grep` and `sed` commands.  


The following code searches for each instance of the word license (with upper, lower, or mixed cases):  

```bash
grep -i "license" GPL-3
```

By the end of this module, I now have a clear understanding of character encoding, learning how computers store and handle all text. I mastered essential tools like `grep` and `sed`, which I can use for precise searching and editing of data in the terminal. The best part was learning to connect commands to create powerful, efficient pipelines for complex tasks.

---
## Module 3: Scripting, Configuration Files and Installing Programs

we  learnt to create and use scripts to automate complex tasks, moving beyond individual commands. We were also introduced to the crucial concept of UNIX environment variables to control system behavior. Finally, we set up our own configuration file to easily manage and maintain our custom system settings.  

![Git](https://www.explainxkcd.com/wiki/images/4/49/universal_install_script.png)

In the following code, we create a bash script that takes one argument, an English adjective and prints its comparative form.

```bash

#!/bin/bash

if [ $# -eq 1 ]; then
    adjective=$1
    comparative="${adjective}er"
    echo "$comparative"
else
    echo "Usage: $0 <adjective>"
fi
```

I can now write simple scripts to automate many commands at once, which makes complex tasks much easier to handle. I learned how to customize my terminal by changing environment variables and saving personal shortcuts in configuration files. I gained the ability to install new software using system tools like `apt-get` and learned how to set up virtual environments for my Python projects.  

---

## Module 4: Using ssh, scp and Version Control

This module introduces version control, a fundamental practice for all projects. This system is essential for reverting to past work and for coordinating changes when multiple people are working together. We will explore the most popular tools in this space: the version control system **_Git_** and its primary host platform,**_GitHub_**.  

```bash
$ scp examplefile yourusername@yourserver:/home/yourusername/
```
The scp command above will transfer the file "examplefile" to the directory "/home/yourusername/" at the server "yourserver".   

I learned how to use git add, git commit, and git push to track and share changes:  

Command | Description 
--- | ---
`git add .` | Stage all modified files
`git commit -m "message"`| commit files
`git push origin main`| Upload changes to GitHub


I learnt how to manage running programs (processes) and how to connect and securely copy files to and from remote servers.I successfully set up Git and GitHub, mastering the workflow of saving, committing, and uploading my project changes online. I can now use branches to manage separate features and confidently undo mistakes by reverting my code to an earlier version.  

