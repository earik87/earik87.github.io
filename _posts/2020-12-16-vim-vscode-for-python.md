# Vim vs Visual Studio Code for Python

I started a course on Udemy about data structures and algorithms in python. There are tons of things to learn this course. Therefore, I needed something easy to use. I started with Vim and then switched to Visual Studio Code (VS Code). In this blog, I will elaborate my experience on both editors and why I switch to VS Code later.

# Vim
Vim (Vi-IMproved) is a highly configurable text editor. It is developed by Bram Moolenaar. The first stable release was in 1991, since then it became very popular among the programmers. I am familiar with with Vim due to my job. This led me to start with Vim for python development. 
Let's run the terminal first.

I usually keep my python files in a special directory. For this, going to the target directory by typing `cd foldername` is a pain. Alias is a nice trick which allows an easy access to the target directory with one word. I added following line into *.bash_profile* file.

`alias pythonfiles='cd ~/"Google Drive"/py_course'`

When I type `pythonfiles` into the terminal, then current directory will be `~/"Google Drive"/py_course'`. When I learned this, it saved me a lot of time. 

Next thing, we want to create our python file. For this, you can just open vim by typing `vim` in the terminal. Then, Vim will be running in the terminal window. When you finish writing or editing your python code, to save it, go to command mode <:> then type `w code.py`. This command will write a new file in python syntax in current directory. To open the same file, just type `vim code.py`. I highly recommend you to do vimtutor before stepping into those codes. Because you need to know basics first. 

When a python file open in Vim, I realized I need terminal next to it. Because, constantly switching between Vim and terminal is annoying. For this there is a nice trick. 

Open the file in Vim. Then type `:term`. This will open terminal inside Vim. After this you can move terminal up or down by using Ctrl + w + up/down. I personally prefer terminal in the bottom of the code. 

This is how Vim and terminal look together.
![terminal inside vim](vim_term.png)

It is also possible to align terminal horizontally. For this, `rightb vert term` will place terminal on the right side of Vim. 

![terminal inside vim](vim_term_h.png)

This is a neat initial Vim setup for basic Python source code editing. Vim has python syntax highlighting which works great. The big advantage of Vim is its speed. Nothing can beat it. As I said, you have to know how to configure it for the first time. 

Issues with Vim;

I did not go very far with Vim especially for Python development. Reason is my time is precious, and I want to focus on my course not the editor itself. I am pretty sure one can make use of Vim as a Python development environment but I do not have that time and energy. That's why in the second section of this blog post, I will mention Visual Studio Code which is my to-go development tool. 

# Visual Studio Code

I used Vim for the course assignments for a while but to be honest, I could not be stick to it. I needed something more than Vim. I want to have auto-completion and debugger with the editor at least. I know these might be possible with Vim but I do not want to spend my time on it. That's why here VS Code comes for help. 

VS Code is a product of Microsoft which has been released in 2015. It is a very ight-weight developer environment tool. In contrast to Vim, it comes within great built-in features; debugger, intellisense, complete Git integration. It has marketplace where you can find any kind of extensions for your needs. It has been selected the most used environment, according to stackoverflow survey in 2019.  

![stackoverflow survey 2019](so_survey_2019.png)

For my own VS code setup, I added Python and Vim extensions from marketplace. Python extension brings debugging environment which is super useful to use. On the other hand, I use Vim extension to have the power of Vim movements and modal text editing. Combination of Vim philosophy plus the easiness of VS Code is my to-go setup for development in Python.

![vscode setup](vscode_setup.png)