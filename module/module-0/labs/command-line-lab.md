# Command Line Lab

# Intro
This lab will be an exercise to help further your understanding of the command line. The first thing you will want to do is make sure you have Git (for windows especially, the git bash terminal) installed on your computer.
If you do not have git installed yet, [here is a guide.](https://www.siteground.com/tutorials/git/windows-installation/)

# Starter Code
If you're using a mac or linux machine, you can just open a terminal and start the lab. If you are using a windows machine you will need to open a git bash terminal and start from there.

*Note: If you do come across something not covered by the resources attached to this module, follow these steps.*
  1. *Try looking your question up on google, chances are extremely high that you are not the first person to have this question.*
     * _After you have tried google for at least 10 minutes, try asking your question in the tech questions area on slack. In your question you should include a description of the issue (try including a stack trace if it's a hard error type of issue), everything you have tried to resolve the issue, and be prepared to provide a code snippet._
  2. *If you feel this issue should be covered in the resource document, please let one of the admins know and they will look into it.*

This exercise is going to take you through some of the basic commands of the terminal. Before doing this exercise, you should already know how the following commands work:
  1. ls
  2. cd
  3. pwd
  4. mkdir
  5. rm
  6. cp
  7. mv

# Exercise
**(Replace all occurences of <your_name> with your first name)**
  1. Open your terminal and change directories to your home directory if you are not already there. (The path you want is simply `~`)
  2. Make a directory and call it `CommandLineLab<your_name>`.
  3. Navigate into the directory you just created.
  4. Create a file and call it `hello-world.txt`.
  5. Now open the newly created file in your text editor of choice. Add the lines `Hello World!`, then save and close the file.
  6. Back in your terminal (if you left it for your text editor/IDE), let's rename the file to `hello-<your_name>.txt`.(**no cheating, use the terminal!**)  
  7. Now lets create a copy of that file, but with yet another new name, let's call this one `<your_name>.txt`.
  8. List out the contents of your current directory. See how we have 2 files now? Lets fix that...Delete `hello-<your_name>.txt`.
  9. Now We're going to run two commands that might not look familiar to you, we are going to append some text to `<your_name>.txt`.
     * Run the following command (don't worry if you have no idea what this is doing, there is an explanation below) `echo $(pwd) >> <your_name>.txt`.
       * Let's break the above command into pieces. The first part, `echo` is telling your terminal (also known as a shell) to print out the stuff after it as standard output. The next part, `$(pwd)` is telling your terminal to run the command `pwd` (Think of it this way, `$(pwd)` is being replaced in the `echo` command with its output). The final part, `>> <your_name>.txt` is actually appending the output of the first two parts into your file that we created above. So if you open `<your_name>.txt` and look at the contents you should see our 'Hello World!' and then a line below that should be the output of `pwd`.
     * Now let's run this command, `echo $(ls) >> <your_name>.txt`. Based off the previous commands explanation can you figure out what this command is doing?
  10. (Bonus) Open your file <your_name>.txt back up, and in your own words, breifly explain what each of the commands you used during this lab does. (Bonus X2) Include the last two commands in your explanations, `echo $(pwd) >> <your_name>.txt` and `echo $(ls) >> <your_name>.txt`.

Assuming everything went well, you now have a file called `<your_name>.txt` with "Hello World!" and the output of a `pwd` command and a `ls` command. Make sure you keep the file and folder that contains it, when we complete the git and github lab you will be able to submit it for review!
