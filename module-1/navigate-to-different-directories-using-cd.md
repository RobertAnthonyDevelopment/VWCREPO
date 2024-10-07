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

![Image of Sixteen](module-1-images/navigate-to-different-directories-using-cd-images/Sixteen.png)

## Common Scenarios:
This command is useful when you need to backtrack to a higher-level directory in your file structure.

### Move to the Parent Directory (cd ..)
You can move up one level in the directory structure using the .. symbol.

