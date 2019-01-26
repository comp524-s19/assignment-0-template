---
title: Assignment 0
author: COMP 524 - Spring 2019
documentclass: article
geometry: margin=1.5in
...


# Overview
The intent of this assignment is to test that all the pieces you need for future assignments work properly. We will use GitHub Classroom to privately store your coursework, and Gradescope for autograding. We also intend for you to be able to complete all your assignments inside of the virtual machine. If you have not yet setup your virtual machine, please refer to the "Virtual Machine Setup Instructions" document on the course website.

![High-level view of the course workflow and major systems you may deal with](comp-524-workflow.pdf)

# Initialize GitHub Classroom
You first need to join our GitHub Classroom and Assignment 1 on there via this link: https://classroom.github.com/a/SZduEcG5). It will first prompt you to login to or create a GitHub account; we recommend using an existing GitHub account if you have one. After this, accepting the assignment will create a private repository which you can store your code to.

# Clone the Repository, Add a File, Commit, and Push
We use Git to interface with GitHub and use a number of other UNIX tools to move around and edit files in our virtual machine. Here's the essential list of commands and git subcommands that you will need (replace the words in <tags> with the values specific to you):

- `ls` to list files in your current directory
- `cd <something>` to change your location to the `<something>` directory
- `nano <file name>` to open a text editor on either an existing file or on one you want to create
- `git clone <some URL>` to clone a repository from `<some URL>` to your machine
- `git add <some file name>` to add a file to your next Git commit
- `git commit -m "<commit description>"` to commit all previously `git add`ed files with some description
- `git push` to send all your `git commit`ed code back to the online repository you originally `git clone`d from

You can do all the following steps using just the above commands unless otherwise noted:

1. Open up the directory where you setup your VM with Vagrant then run `vagrant up` and `vagrant ssh` to get back to the console inside the VM that you previously set up
2. Clone the URL `https://github.com/comp524-s19/assignment-0-[YOUR GITHUB USERNAME].git`, replacing the `[YOUR GITHUB USERNAME]` part of that appropriately
3. Move to the directory git created
4. Create a new file named `assign0.txt` with the text "Hello!"
5. Commit and push `assign0.txt` with git. Use whatever commit description you would like. (You can check this worked by looking at the state of your repository on the GitHub website.)

# Join and Submit to Gradescope
First join Gradescope using course code `9JKRV7`. Once joined, you can submit your work from GitHub to the Gradescope autogreader. To do so, open Gradescope and find "Assignment 0" under the COMP 524 class. The first time you attempt to upload your work from GitHub to Gradescope you will need to authorize Gradescope to have access to your GitHub repositories. **Important:** when authorizing Gradescope with GitHub, make sure to press the "Grant" button for the comp524-s19 organization. Otherwise, Gradescope will not have access to your assignment repositories and you will have to reset the authorization in GitHub (<https://help.github.com/articles/reviewing-your-authorized-integrations/>) before refreshing and reauthorizing correctly in Gradescope. Once authorized, you can create a submission by selecting your private repository from the Repository selector and `master` from the branch selector. Once uploaded, the autograder should run with feedback shortly. Assuming it runs without finding any problems, congratulations! Your envirnoment is ready to go for future, more substantial assignments. (At this point, you may also want to consider running `exit` and `vagrant halt` to power off your virtual machine.)
