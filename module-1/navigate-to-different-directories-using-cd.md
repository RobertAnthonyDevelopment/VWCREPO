# Navigate to different directories using cd

## Introduction
Basic directory navigation is an essential skill when working in the terminal. The “cd” command which stands for "change directory" allows you to move between directories and access files or programs in different locations on your system. This section covers the simplest forms of the cd command, explaining how to navigate directly to specific directories.

## Basic Usage:

### Find Specific Directory:
This command demonstrates how to navigate to a specific directory using the full (absolute) path, which is necessary when you're not sure where you are in the file system.
- cd /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

![Image of One](module-1-images/navigate-to-different-directories-using-cd-images/One.png)

![Image of Two](module-1-images/navigate-to-different-directories-using-cd-images/Two.png)

### List the Contents of the Directory:
After navigating to a directory, you can use ls to list the contents of that directory
and confirm you are in the right place.
- ls /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

![Image of Three](module-1-images/navigate-to-different-directories-using-cd-images/Three.png)

![Image of Four](module-1-images/navigate-to-different-directories-using-cd-images/Four.png)

## Advanced Options:

### Demonstrating the `ls` Command with Absolute Path

### Navigate to the Directory:
- cd /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

### Basic ls Command:
- ls This will display all the non-hidden files and directories located within cdnavpracticesub.

![Image of Twenty Nine](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Nine.png)

![Image of Thirty](module-1-images/navigate-to-different-directories-using-cd-images/Thirty.png)

### List All Files (Including Hidden Files):
- ls -a /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This command will list all files, including hidden ones, within the cdnavpracticesub directory.

![Image of Thirty One](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20One.png)

### Long Listing Format (-l flag):
- ls -l /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
The output will display file types, permissions, number of links, owner, group, file size, and the last modified time.

![Image of Thirty Two](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Two.png)

### Long Listing with Hidden Files:
- ls -la /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This is useful when you want detailed information on all files, including hidden ones.

![Image of Thirty Three](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Three.png)

### Listing Only Directories:
- ls -d /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This will output the directory name without listing the files inside it.

![Image of Thirty Four](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Four.png)

### Multiple Directory Listing:
- ls -d -l /Users/robertclemons/Desktop/cdnavpractice /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This will list details of the cdnavpractice and cdnavpracticesub directories.

![Image of Thirty Five](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Five.png)

### Displaying Entries in Multiple Columns:
- ls -C /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This shows the contents of the directory in multiple columns.

![Image of Thirty Six](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Six.png)

### Displaying Comma-Separated Output:
- ls -m /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This will output the contents of the directory in a single line, separated by commas.

![Image of Thirty Seven](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Seven.png)

### Checking File Types and Permissions:
- ls -l /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This will show:
- d: Directory
- -: Regular file
- l: Symbolic link

![Image of Thirty Eight](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Eight.png)

### Listing Files with Extended Security Information:
- ls -e /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This provides an additional 11th character in the output to indicate if extended security information is present.

![Image of Thirty Nine](module-1-images/navigate-to-different-directories-using-cd-images/Thirty%20Nine.png)

### Listing Block Size:
- ls -s /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub
This will show the total size of blocks for files in the directory.

![Image of Forty](module-1-images/navigate-to-different-directories-using-cd-images/Forty.png)

### Practical Examples:
- ls -a /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

- ls -d -l /Users/robertclemons/Desktop/cdnavpractice /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

![Image of Forty One](module-1-images/navigate-to-different-directories-using-cd-images/Forty%20One.png)

### More Resources:
To learn more about the ls command and its options, use the manual:
- man ls

![Image of Forty Two](module-1-images/navigate-to-different-directories-using-cd-images/Forty%20Two.png)


### Switch to the Previous Directory (cd -):
Switching between directories with cd - is useful when you're frequently moving between two working directories. For example, if you’re editing files in one directory and testing code in another, cd - saves time by toggling between the two without having to retype the full paths each time. This is a very useful feature that allows you to toggle between two directories.

- cd /Users/robertclemons/Desktop/cdnavpractice 

- cd -

![Image of Five](module-1-images/navigate-to-different-directories-using-cd-images/Five.png)

![Image of Six](module-1-images/navigate-to-different-directories-using-cd-images/Six.png)

![Image of Seven](module-1-images/navigate-to-different-directories-using-cd-images/Seven.png)

### Creating Symbolic Link
A symbolic link is like a shortcut that points to another directory or file. You can create it to easily access a directory without navigating the full path every time. Symbolic links act as shortcuts to directories or files. They are particularly useful when you need to access a directory or file located deep within a directory structure. By creating a symbolic link, you can place a shortcut in a more convenient location. You can easily access the original directory without typing the full path, saving you time and effort when navigating complex file systems.

- ln -s /Users/robertclemons/Desktop/symboliclinkexample /Users/robertclemons/ Desktop/cdnavpractice/cdnavpracticesub/ExampleLink

- ls -l /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

- cd /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub/ExampleLink

![Image of Eight](module-1-images/navigate-to-different-directories-using-cd-images/Eight.png)

![Image of Nine](module-1-images/navigate-to-different-directories-using-cd-images/Nine.png)

![Image of Ten](module-1-images/navigate-to-different-directories-using-cd-images/Ten.png)

### Navigate Through the Physical Directory, Ignoring the Symbolic Link
The -P flag forces the terminal to navigate the physical directory, ignoring symbolic links. This can be useful if you want to avoid being redirected through a symbolic link.

- cd -P /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub/ ExampleLink

- pwd

![Image of Eleven](module-1-images/navigate-to-different-directories-using-cd-images/Eleven.png)

![Image of Twelve](module-1-images/navigate-to-different-directories-using-cd-images/Twelve.png)

### Remove Symbolic Link
rm -r /Users/robertclemons/Desktop/symboliclinkexample

![Image of Thirteen](module-1-images/navigate-to-different-directories-using-cd-images/Thirteen.png)

![Image of Fourteen](module-1-images/navigate-to-different-directories-using-cd-images/Fourteen.png)

### Remove ExampleLink Folder
rm /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub/ExampleLink

![Image of Fifteen](module-1-images/navigate-to-different-directories-using-cd-images/Fifteen.png)

![Image of Sixteen](module-1-images/navigate-to-different-directories-using-cd-images/sixteen.png)

## Common Scenarios:
This command is useful when you need to backtrack to a higher-level directory in your file structure.

### Move to the Parent Directory (cd ..)
You can move up one level in the directory structure using the .. symbol.

![Image of Seventeen](module-1-images/navigate-to-different-directories-using-cd-images/Seventeen.png)

### Return to the Home Directory (cd ~):
Using ~ (tilde) is a shortcut to go back to your home directory, regardless of your current location.

![Image of Eighteen](module-1-images/navigate-to-different-directories-using-cd-images/Eighteen.png)

### Navigating Multiple Levels Up (cd ../../)
You can combine multiple .. to move up several directory levels in one go.

![Image of Nineteen](module-1-images/navigate-to-different-directories-using-cd-images/Nineteen.png)

## TASK 3 Continued: Absolute vs. Relative Path

An absolute path starts from the root of the file system and is always the same, while a relative path is based on your current location in the file system. Here’s how you would use each. Absolute paths are useful when you need to navigate to a specific directory from anywhere in the file system. They start from the root (/) and provide the full location of the directory. Relative paths, on the other hand, depend on your current location in the system. They are shorter and more convenient when you're already near your destination directory, as they save you from typing the full path.

### Scenario 1: You Are in /Users/robertclemons

### Absolute Path Example:

Let’s say you want to go to the cdnavpracticesub directory located at /Users/ robertclemons/Desktop/cdnavpractice/cdnavpracticesub. You would use the absolute path to get there, regardless of where you are in the filesystem.

- cd /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

![Image of Twenty](module-1-images/navigate-to-different-directories-using-cd-images/Twenty.png)

### Relative Path Example:
Now, if you're already in /Users/robertclemons, and you want to go to
cdnavpracticesub, you can use a relative path. 

- cd Desktop/cdnavpractice/cdnavpracticesub

![Image of Twenty One](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20One.png)

### Scenario 2: You Are in /Users/robertclemons/Desktop

### Absolute Path Example:
- First, the user uses an absolute path to go to the Desktop folder by typing: cd /Users/robertclemons/Desktop

- Then: Even though you’re already in the Desktop folder, you can still use an absolute path to get to cdnavpracticesub.

- cd /Users/robertclemons/Desktop/cdnavpractice/cdnavpracticesub

![Image of Twenty Two](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Two.png)

### Relative Path Example:
- First, the user uses an absolute path to go to the Desktop folder by typing:
cd /Users/robertclemons/Desktop
- Then, instead of typing the full absolute path again, the user uses a relative path to navigate to cdnavpracticesub:
cd cdnavpractice/cdnavpracticesub

![Image of Twenty Three](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Three.png)

## Troubleshooting:
### "No such file or directory" Error
### Issue:
This error occurs when you try to navigate to a directory that doesn't exist or you’ve made a typo in the directory name.

### Example of Bad Command:
(base) robertclemons@Ricky-Spanish ~ % cd /Users/robertclemons/Desktop/ nonexistentfolder

### This will result in:
cd: no such file or directory: /Users/robertclemons/Desktop/nonexistentfolder (base) robertclemons@Ricky-Spanish ~ %

### Solution:
Double-check the spelling and ensure that the directory actually exists by listing the contents of the parent directory.
Run “ls /Users/robertclemons/Desktop” to list the contents and confirm the directory exists. If it doesn't, double-check the spelling or navigate to a different location.

![Image of Twenty Four](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Four.png)

### Navigating Directories with Spaces

When directory names contain spaces, you need to take special care, as spaces can cause issues in the command line.

### Issue:
cd /Users/robertclemons/Desktop/My Folder

### Example of Bad Command:
(base) robertclemons@Ricky-Spanish ~ % cd /Users/robertclemons/Desktop/nonexistentfolder

### This will result in:
cd: string not in pwd: /Users/robertclemons/Desktop/My

### Solution:
There are two ways to handle directories with spaces:

- Use quotation marks around the path:
  cd "/Users/robertclemons/Desktop/My Folder"

- Escape the spaces with a backslash (\):
  cd /Users/robertclemons/Desktop/My\ Folder

![Image of Twenty Five](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Five.png)

### Clearing Terminal and Checking Your Current Location
If you’ve run several commands and the terminal is cluttered, you can clear the screen to start fresh. This doesn't affect your location, but you can use pwd afterward to confirm where you are.
### Issue:
Sometimes, you may not know where you are in the file system, which can make it difficult to understand why cdcommands aren’t working as expected.
### Solution:
Use the pwd (print working directory) command to confirm your current location:
Type: “clear” Press the “Enter” key

![Image of Twenty Six](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Six.png)

This will be the result:

![Image of Twenty Seven](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Seven.png)

Use the “pwd” (print working directory) command to confirm your current location:

![Image of Twenty Eight](module-1-images/navigate-to-different-directories-using-cd-images/Twenty%20Eight.png)

### CONCLUSION
In conclusion, mastering the cd command is essential for effective navigation in Unix-like operating systems. From basic usage to more advanced techniques like switching between directories, using symbolic links, and troubleshooting common issues, understanding how to work with directories is a critical skill for anyone working in the terminal. With these tools, you will be able to navigate the file system efficiently, troubleshoot errors, and streamline your workflow.

### References 
[How To Use 'CD' 'Change Directory'](https://www.linode.com/docs/guides/how-to-use-cd/)
