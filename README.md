# Command Line Basics

### Let's learn how to use your terminal.

Programmers use the terminal to navigate and run commands on their computers. Before the invention of the mouse and the Graphical User Interface (GUI), the terminal was the only way to interact with your computer! For many of the labs that we'll be working through, you'll be asked to use your terminal to do the same. 		


## *pwd* - print working directory
The first thing we need to understand when we use the terminal is what directory (another word for folder) working in right now. We can figure this out by typing 'pwd' - this will list the folder that we are currently 'situated in' (you can think of directories as rooms that you can move in and out of)

	[10:33:02] ~
	// ♥ pwd
	/Users/EmilyMott
	[10:33:04] ~
	// ♥

When I type `pwd` into my command line, it tells me the full path of my current directory - `/Users/EmilyMott`. This is my root directory, as noted by the `~` in the prompt.

## *ls* - list
Let's say I'm in a directory, and I want to know what other files and directories are inside it. We can use the `ls` command to list all of the material that we have access to.

	[10:35:28] ~
	// ♥ ls
	Applications	Public
	Books			Google Drive
	Code			Library			
	Desktop			Movies			
	Documents		Music
	Downloads		Pictures
	[10:35:29] ~
	// ♥

By typing `ls` I can see that I have a lot of directories inside of my root directory that I can work with. Next, let's learn how to access these directories.

## *cd* - change directory

A **directory** is another word for a folder, which we typically use on our computers to organize files. The organization is exactly the same here - in fact, we can access any directory that currently exists on your computer using the command line.	Above we saw that within `~` I have a folder called `Code`. Let's access that folder by typing `cd` and the name of the directory.

	[10:23:40] ~
	// ♥ cd Code
	[10:23:53] Code
	// ♥

As we can see above, after we `cd` into the `Code` directory, our prompt changes from `~` to `Code`. Now we're in the Code directory!		
If we want to go back up one level we use the command ``cd ..``. 

	[10:28:27] Code
	// ♥ cd ..
	[10:28:32] ~
	// ♥

This brings us back up to the top directory.		
This is great for directories that already exist, but what if we want to make one?

## *mkdir* - make directory

We can also create directories in the command line. Let's say I'm in the `Code` directory and I want to create a `labs` folder to store all of my work. We can use `mkdir` followed by the directory name to create a new directory.

	[10:41:00] Code
	// ♥ mkdir labs

We can't tell right away if this command worked. But if we use our `ls` command, we should be able to see all the directories that exist inside `Code`.

	[10:41:00] Code
	// ♥ mkdir labs
	[10:41:17] Code
	// ♥ ls
	labs

We can `cd` into labs now as well!

	[10:41:00] Code
	// ♥ mkdir labs
	[10:41:17] Code
	// ♥ ls
	labs
	[10:42:18] Code
	// ♥ cd labs


## *touch* - create a file

We can make a directory - but what about an actual file? This is done with the `touch` command. Let's stay inside the `labs` directory and make a new lab file.

	[10:44:20] labs
	// ♥ touch new_lab.rb

Now if we `ls` we can see that the file `new_lab.rb` exists.

	[10:44:20] labs
	// ♥ touch new_lab.rb
	[10:44:28] labs
	// ♥ ls
	new_lab.rb

You're officially a command line wizard!
