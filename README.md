# linux-fundamentals-sheet

Linux fundamentals notes for cybersecurity and ethical hacking.

## Contents
- File system navigation
- File and directory operations
- Permissions and ownership
- Searching and filtering files
- Text processing
- Bash basics

File System Navigation & Inspection
Navigation
•	pwd “Print working director”: Command display the file where I work.

•	cd “change directory”: command that allow to move between folders.

Listing & File Information
•	ls “List”: show files and directories.
Options: 
▶	-l:  shows the long format of files.
▶	-A: shows the hidden files.
▶	-S: shows files and directories along with their sizes

•	File: Command that determines the type of file.

File & Directory Management
Links
•	ln “Link”: Command creates links to files or directories. Options of ln:
▶	-s: creates a soft link.
▶	-f: Force overwrite if the link already exists.
▶	-v: shows what’s happening step by step.
▶	-n: don’t dereference soft link.
▶	-t: treat target as file.


Copy, Move & Remove
•	cp “copy”: Command that copy files or directors from one location to another.
Options of cp:
▶	-i: prompts before overwriting an existing file.
▶	-r: copies directories and their contents recursively.
▶	“directoryName1” /* “directoryName2”: Copy all contents of the attend folder

•	mv “move”: command used to move or rename files and directories.
Options of mv:
▶	-i: prompts before overwriting an existing file.
▶	-v: Display detailed information about what the command is doing.

•	Mkdir “make directory”: Command that create a new directory or multiple directories
.
•	Touch: command used to make file.

•	rm “remove”: Command that removes files and directories.
Options of rm:
▶	-i: prompts before overwriting an existing file.
▶	-r: Removes directories and their contents recursively.




Text Editing & Viewing
Text Editors
•	nano: is a command allows you to quickly create, view, and edit text files directly from the terminal.

File Content Display
•	cat: Is used to display smalls text files without opening new page.

Command Discovery & Documentation
Command Identification
•	type: used to determine the type of command.
•	which: used to determine the location of command.

Help & Manuals
•	Help: used to show all information about the shell built-in commands.

•	apropos: Searches the man page database for commands or topics related to a keyword.

•	Man “manual”: used to show user manual of any command has manual.



Permissions & Ownership
Permissions
•	chmod: command used to change permissions of files and directories. And it supports changing permissions using numeric (octal) mode.

Ownership
•	whoami: command used to show the current user name.
•	chown: command used to change the owner of file or directory.
•	chgrp: used to change the owner group of a file or directory.

ACL (Access Control Lists)
•	getfacl: command used to show permissions of a file or directory.
•	setfacl “using with groups or others” : used to change permissions of a file or directory for users or groups.

Searching & File Discovery
File System Search
•	find: Command used to search for files and directories based on various conditions within the filesystem in real time.

•	-type: match files based on their type, such as regular files, directories, or symbolic links.

•	-name: match files and directories based on their name or a specified filename pattern.

•	-size: match files according to their size.

•	-user: match files owned by a specific user.

•	-exec: Executes a command on each found file.

•	-delete: Deletes files found by find.


Text Processing & Comparison
Sorting & Filtering
•	Sort: command used to sort command output or text file content.
Options of sort:
▶	-r: used to sort UP to Down.
▶	-o: option used to save sorted output to a file.

•	Uniq: command used to remove or filter duplicate lines from sorted text.
Options of uniq:
▶	-u: option used to display only unique lines from sorted text.
▶	-c: option used to count how many times each line appears in sorted text.


File Comparison
•	comm: command used to compare two sorted files line by line.
Options of comm:
▶	- "column num": hide lines unique to the selected line.

•	diff: command used to show differences between two files line by line.
Options of diff:
▶	-i: option used to compare files while ignoring case differences.
▶	-c: option used to show differences with surrounding context lines.

Text Extraction
•	cut: command used to extract specific columns or fields from text. Is require OPTIONS
Options of cut:
▶	-c: used to select specific character positions from each line.
▶	-f: option used to select specific fields from text separated by a delimiter.
▶	-d: option used to specify the delimiter that separates fields in text.




Shell Operators & Expansions
Redirection & Process Control
•	<: Redirects input from a file to a command.

•	<<: Provides multi-line input in the terminal until a delimiter.

•	| (pipeline): shell operator that uses pipes to connect commands.

•	& (Background Jobs): processes running in the background that allow using the terminal during execution.

Wildcards
•	Wildcard: symbols used to match multiple files or directories by pattern.

•	* (asterisk): used to match any number of characters.

•	? (question mark): used to match one character only.

•	(file*.txt): matches files with the same name pattern.

•	[ ](sets): used to match one character from a specific set.

•	[!]: used to match one character NOT in the specified set.




Expansions & Quoting
•	Brace Expansion: matches patterns inside { } and expands them into multiple values.

•	~ (Tilde Expansion) : expands to user’s home directory.

•	Parameter Expansion: shell feature sed to expand and manipulate variables before command execution.

•	" ": Allows variable and command expansion.

•	' ': Prevents all expansions (literal text).

•	\ (Backslash): Used to prevent the shell from interpreting the next character.
