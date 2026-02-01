## File System Navigation & Inspection

### Navigation
- `pwd` “Print working director”  
  Command display the file where I work.

- `cd` “change directory”  
  command that allow to move between folders.

### Listing & File Information
- `ls` “List”  
  show files and directories.

Options of ls:
- `-l` shows the long format of files.
- `-A` shows the hidden files.
- `-s` shows files and directories along with their sizes.

- `file`  
  Command that determines the type of file.

---

## Links

- `ln` “Link”  
  Command creates links to files or directories.

Options of ln:
- `-s` creates a soft link.
- `-f` Force overwrite if the link already exists.
- `-v` shows what’s happening step by step
- `-n` don’t dereference soft link
- `-t` treat target as file

---

## File & Directory Operations

- `cp` “copy”  
  Command that copy files or directors from one location to another.

Options of copy:
- `-i` prompts before overwriting an existing file.
- `-r` copies directories and their contents recursively.

- `mv` “move”  
  command used to move or rename files and directories.

Options of mv:
- `-i` prompts before overwriting an existing file.
- `-v` Display detailed information about what the command is doing.

- `rm` “remove”  
  Command that removes files and directories.

Options of rm:
- `-i` prompts before overwriting an existing file.
- `-r` Removes directories and their contents recursively.

- `mkdir` “make directory”  
  Command that create a new directory or multiple directories.

- `touch`  
  command used to make file

---

## File System Tree

Unix-like OS using hierarchical directory structure Method to organized flies.

- Root  
  The First Folder in the tree.

- Current working directory  
  the Folder that you are in.

- Parent directory  
  each folder contains folders or files.

- Brach  
  each folder or File inside folder.

---

## Permissions & Ownership

Types of files:

- Regular File `-`  
  All files that contain data

- Directory `d`  
  Folders

- Character device `c`  
  A device that sends and receives data one piece at a time, like typing on a keyboard.

- Block device `b`  
  A device that stores data and reads or writes it in large chunks, like a hard disk.

- Pipe `p`  
  Allows communication between two processes, where the output of one process becomes the input of another.

- Socket `s`  
  Are files used for communication between running programs to transfer data on the same device or over the network.

- Soft link `l`  
  Command creates links to files or directories.

Types of Permission:

- Read `r`  
  Reading files

- Write `w`  
  Writing on file

- Execute `x`  
  Executing the file

Grant to:
- User
- Group
- Public

---

## Permission Commands

- `chmod`  
  command used to change permissions of files and directories.

- `whoami`  
  command used to show the current user name.

- `chown`  
  command used to change the owner of file or directory.

- `chgrp`  
  used to change the owner group of a file or directory.

---

## Searching Files

- `find`  
  Command used to search for files and directories based on various conditions within the filesystem in real time.

Options:
- `-type`  
  match files based on their type

- `-name`  
  match files and directories based on their name or a specified filename pattern.

- `-size`  
  match files according to their size.

- `-user`  
  match files owned by a specific user.

Actions:
- `-exec`  
  Executes a command on each found file.

- `-delete`  
  Deletes files found by find.

---

## Text Processing

- `sort`  
  command used to sort command output or text file content.

Options:
- `-r` used to sort UP to Down.
- `-o` option used to save sorted output to a file.

- `uniq`  
  command used to remove or filter duplicate lines from sorted text.

Options:
- `-u` option used to display only unique lines from sorted text.
- `-c` option used to count how many times each line appears in sorted text.

- `comm`  
  command used to compare two sorted files line by line.

- `diff`  
  command used to show differences between two files line by line.

- `cut`  
  command used to extract specific columns or fields from text.

Options:
- `-c` used to select specific character positions from each line.
- `-f` option used to select specific fields from text separated by a delimiter.
- `-d` option used to specify the delimiter that separates fields in text.

---

## Bash Basics

Wildcard:
symbols used to match multiple files or directories by pattern.

- `*` asterisk
- `?` question mark
- `[ ]` sets
- `[!]` NOT in the specified set

Brace Expansion:
matches patterns inside `{ }` and expands them into multiple values.

---

## Streams & Pipes

Types of streams:
- Stdin `0`
- Stdout `1`
- Stderr `2`

- `|` pipeline  
- `&` Background Jobs
