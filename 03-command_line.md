# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > Command Line Cheat Sheet:
    * show current working directory path = pwd
    * creating a directory = mkdir
    * deleting a directory = rmdir
    * creating a file using `touch` command = touch file.txt
    * deleting a file = rm
    * renaming a file = mv oldfilename newfilename
    * listing hidden files = ls -a
    * copying a file from one directory to another = cp source destination
    * print a file = cat
    * look at enviornment = env
    * global regular expression print = grep

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > `ls` = list files and directories  
    `ls -a` = list all hidden files and directories  
    `ls -l` = list all files and directories in long format  
    `ls -lh` = long listing with Human readable files sizes  
    `ls -lah` = long listing with all hidden files and Human readable file sizes  
    `ls -t` = long listing organized by time  
    `ls -Glp` = long list, doesn't print group name, append / to directories  
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > ls -m = displays names as comma separated list  
    ls -o = long list but excludes group name  
    ls -r = displays files in reverse order  
    ls -R = displays subdirectories  
    ls -x = displays files as rows  

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > 'xargs' is a command used to convert inputs from STDIN into arugments to command. An example is xargs find -name, where you would specify the name of the file as an input.

 


