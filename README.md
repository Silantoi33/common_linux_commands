# Common_linux_commands
Common commands that are used in windows subsystem for linux (wsl)

1. ### Opening Ubuntu in WSL
After you’ve installed Ubuntu in WSL, you can open it by typing wsl in your Windows terminal or search "Ubuntu" in your start menu. Once opened, you'll see a terminal window where you can enter Linux commands.

2. ### What is a Directory?
A directory is like a folder in Windows, where you store files and other directories. Think of it as a way to organize your data.

Command: `mkdir` is used to create a directory (folder).
Example:
Let's create a directory called practice.
```
mkdir practice
```
This creates a folder named "practice" where you can store files or other directories.

3. ### Navigating Directories
You are usually in the home directory when you first open Ubuntu. To move into the practice directory, you’ll use the `cd` (change directory) command.

Command: `cd` is used to move into a directory.
Command: `pwd` (print working directory) tells you where you are.
Example:
To go into your new directory, type:
```
cd practice
```
```
pwd
```
You should now be inside the practice directory. You can check your current location with `pwd`.

4. ### Creating Files
Now, let's create some files. There are different ways to do this, but we'll use the `touch` command for simplicity.

Command: `touch` is used to create an empty file.
Example:
Let's create files named fruits.txt and countries.txt.
```
touch fruits.txt countries.txt
```
This creates two empty files called "fruits.txt" and "countries.txt".

5. ### Listing Files in a Directory
To see what files are inside the practice directory, use the `ls` command.

Command: `ls` lists all the files and directories inside the current directory.
Example:
```
ls
```
You should see:
```
fruits.txt  countries.txt
```

5. ### Adding Content to the files we created
We will use `nano` to open the files and manually enter content.

Command:   nano   is a text editor you can use in the terminal.
Example:
To add fruits to fruits.txt:
```
nano fruits.txt
```
Once inside the nano editor, type the following lines:
```
Apple
Banana
Orange
Mango
Grapes
```
To save the file:

Press Ctrl + S (to save)
then
Press Ctrl + X to exit.
Do the same for countries.txt:
```
nano countries.txt
```
Add the following countries:
```
Kenya
Uganda
Tanzania
Ethiopia
Rwanda
```
Then save and exit as before (Ctrl + s, Ctrl + X).

6. ### Viewing File Content
You can now view the content using `cat`.
or if the content is large you can use the command `less` (the content will appear in the text editor, exit with Ctrl-X)

Example:
```
cat fruits.txt
```
```
cat countries.txt
```
7. ### Copying and Renaming Files
Use `cp` to copy files and `mv` to rename or move them.

Example:
Let’s copy countries.txt to nations.txt:
```
cp countries.txt nations.txt
```
To rename nations.txt to world_nations.txt:
```
mv nations.txt world_nations.txt
```
8. ### Removing Files
To delete a file, use the `rm` command.

Example:
```
rm world_nations.txt
```
9. ### Creating Nested Directories and Moving Files
We can create directories inside directories and move files between them.

Example:
Create a `data` directory inside `practice`:
```
mkdir data
```
Move `countries.txt` into `data`:
```
mv countries.txt data/
```
