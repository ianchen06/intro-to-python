# Intro to the Command Line

## What is the Command Line?

The command line, also known as the terminal, shell, or command prompt, is a text-based interface that allows users to interact with their computer. By typing commands, users can perform tasks that would otherwise be done through graphical buttons and menus.

## Why Learn the Command Line?

For programmers and power users, the command line is indispensable. It enables the automation of repetitive tasks, allows for quick execution of complex operations, and provides tools that can significantly speed up workflows.

## How to Use the Command Line

Using the command line involves typing commands into a text-based interface. This allows for direct communication with the operating system to perform a wide range of tasks.

## Common Commands

### Navigating the File System

1. `pwd` - Print Working Directory
2. `ls` - List directory contents
3. `cd` - Change Directory
4. `mkdir` - Make directory

### File Operations

1. `touch` - Create a new file
2. `rm` - Remove files or directories
3. `mv` - Move or rename files or directories
4. `cp` - Copy files or directories

### Viewing and Manipulating File Content

1. `cat` - Concatenate and display file content
2. `less` - View file content one page at a time
3. `head` - Display the beginning of a file
4. `tail` - Display the end of a file
5. `grep` - Search for patterns within files
6. `wc` - Word count (lines, words, characters)
7. `sort` - Sort lines in a file
8. `uniq` - Remove duplicate lines from a file
9. `cut` - Extract columns from a file
10. `paste` - Merge lines from multiple files
11. `tr` - Translate characters
12. `sed` - Stream editor for filtering and transforming text
13. `awk` - Pattern scanning and processing language

## Practice Exercises

### Navigating the File System

1. Use `pwd` to display your current directory, then create a new directory called "projects" using `mkdir`. Finally, change into the "projects" directory with `cd`.
   ```shell
   pwd
   mkdir projects
   cd projects
   ```

2. List all files and directories in your home directory using `ls`. Then, navigate to the parent directory of your current directory using `cd ..`.
   ```shell
   ls ~
   cd ..
   ```

3. Create a directory tree using `mkdir -p` where "projectA" is a directory containing two subdirectories "src" and "bin".
   ```shell
   mkdir -p projectA/{src,bin}
   ```

### File Operations

1. Create a new file named "sample.txt" using `touch`. Remove it using `rm`, and then create it again.
   ```shell
   touch sample.txt
   rm sample.txt
   touch sample.txt
   ```

2. Rename "sample.txt" to "example.txt" using `mv`, then make a copy of "example.txt" named "backup.txt" using `cp`.
   ```shell
   mv sample.txt example.txt
   cp example.txt backup.txt
   ```

3. Create two files "file1.txt" and "file2.txt" using `touch`. Then, remove them both in one command.
   ```shell
   touch file1.txt file2.txt
   rm file1.txt file2.txt
   ```

### Viewing and Manipulating File Content

1. Use `echo` to add some text to "example.txt". Then, display its contents with `cat`.
   ```shell
   echo "Hello, World!" > example.txt
   cat example.txt
   ```

2. Use `head` and `tail` to view the first and last 3 lines of a file named "log.txt".
   ```shell
   head -n 3 log.txt
   tail -n 3 log.txt
   ```

3. Use `grep` to search for the word "error" in "log.txt". Then, use `wc` to count the number of lines in the file.
   ```shell
   grep "error" log.txt
   wc -l log.txt
   ```

4. Sort the contents of "names.txt" alphabetically and remove duplicates using `sort` and `uniq`.
   ```shell
   sort names.txt | uniq
   ```

5. Extract the second column from "data.csv" using `cut`.
   ```shell
   cut -d, -f2 data.csv
   ```

6. Merge the lines of "file1.txt" and "file2.txt" side by side using `paste`.
   ```shell
   paste file1.txt file2.txt
   ```

7. Replace all instances of "hello" with "hi" in "greetings.txt" using `tr`.
   ```shell
   cat greetings.txt | tr 'hello' 'hi'
   ```

8. Use `sed` to delete the first line from "file.txt".
   ```shell
   sed '1d' file.txt
   ```

9. Use `awk` to print the third column of "data.csv".
   ```shell
   awk -F, '{print $3}' data.csv
   ```

These exercises provide practical experience with a range of command-line tools, enhancing familiarity and proficiency with their functionalities.