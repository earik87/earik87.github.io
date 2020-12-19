---
title: "Vim for Python Development"
layout: post
---

I started a course on Udemy about data structures and algorithms in Python. For writing scripts in Python, I needed a text editor. Due to my job, I already had experience on Vim, and decided to use it. 

For those who do not know, Vim (Vi-IMproved) is a highly configurable text editor which is developed by Bram Moolenaar. The first stable release was in 1991, since then it became very popular among the programmers. 

![Stackoverflow Surver in 2019](/assets/images/so_survey_2019.png)

## Alias for quick access to work directory

Aliases are pretty useful to access into your work directory. Since, going to the target directory by typing `cd foldername` is a pain, Alias allows an easy access to the target directory with one word. I added following line into *.bash_profile* file. (Slash in macOS, backslash in Windows).

`alias pythonfiles='cd ~/"Google Drive"/py_course'`

When I type `pythonfiles` into the terminal, then current directory will be `~/"Google Drive"/py_course'`. When I learned this, it saved me a lot of time. 

## Working with Python Files
Next thing, we want to create our python file. For this, you can open Vim by typing `vim` in the terminal. Then, Vim will be running in the terminal window. When you finish writing or editing your python code, to save it, go to command mode then type `w code.py`. This command will write a new file in python syntax in current directory. To open the same file, just type `vim code.py` in the same directory.

When a python file open in Vim, I realized I need terminal next to it. Because, constantly switching between Vim and terminal is annoying. For this there is a nice trick. Open the file in Vim. Then type `:term`. This will open terminal inside Vim. After this you can move terminal up or down by using Ctrl + w + up/down. I personally prefer terminal in the bottom of the code. 

This is how Vim and terminal look together.
![Vim in Terminal Window](/assets/images/vim_term.png)

It is also possible to align terminal horizontally with Vim. For this, `rightb vert term` will place terminal on the right side of Vim. 

![Horizontally aligned Terminal](/assets/images/vim_term_h.png)

These are tips for the starters who want to use Vim for Python files editing. Vim has python syntax highlighting which works great. Vim is a special text editor where you need to learn how to use it. Once you know it, you will be really fast on any kind of text editing.