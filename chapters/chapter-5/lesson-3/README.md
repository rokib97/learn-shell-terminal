# Positional Arguments and Shell Command Operations

## Overview

This project focuses on understanding and practicing the use of positional arguments in shell commands for file and directory management. You'll learn how to navigate directories, view file contents, move files, and list directory contents using basic shell commands.

## Prerequisites

- Basic knowledge of the Linux terminal and command line interface.
- Familiarity with common shell commands like `cd`, `cat`, `mv`, and `ls`.
- A basic understanding of file systems and directory structures.

## Key Concepts

### Positional Arguments in Functions and Commands

Positional arguments are the values passed to a function or command when it's called. In shell commands, these are typically the files, directories, or options provided in the command line.

#### Examples in Shell Commands:

- The `cd` command takes one positional argument: the directory to navigate to.
  ```bash
  cd /home/user/documents
  ```
- The `mv` command takes two positional arguments: the source file and the destination.
  ```bash
  mv file.txt newfile.txt
  ```

### Common Shell Commands

- **`cd <directory>`**: Changes the current working directory.
- **`cat <file>`**: Displays the contents of a file.
- **`mv <source> <destination>`**: Moves a file from the source to the destination.
- **`ls <directory>`**: Lists the contents of a directory.

## Instructions

1. **Navigating Directories**
   Use the `cd` command to move between directories. Ensure you're in the correct directory before executing any file operations.

   ```bash
   cd /path/to/directory
   ```

2. **Viewing File Contents**
   Use `cat` to display the contents of a file. This is helpful for checking what’s inside a file, such as configuration files, logs, or other data.

   ```bash
   cat filename.txt
   ```

3. **Moving Files**
   Use the `mv` command to move files between directories. This command requires two arguments:

   - The file or directory you want to move.
   - The destination where you want to move the file or directory.

   ```bash
   mv source.txt /path/to/destination/
   ```

4. **Listing Directory Contents**
   To confirm a file has been moved or to view the contents of a directory, use `ls`.
   ```bash
   ls /path/to/directory
   ```

## Example Use Case

### Task

- Inspect the contents of a suspicious `key.txt` file in the `worldbanc/public` directory.
- Move the `key.txt` file to a more secure location in the `worldbanc/private/` directory.
- List the contents of the `worldbanc/private/` directory to confirm the file has been successfully moved.

### Commands:

```bash
# Navigate to the 'public' directory
cd worldbanc/public

# Display the contents of 'key.txt'
cat key.txt

# Move 'key.txt' to the 'private' directory
mv key.txt ../private/

# List the contents of the 'private' directory
ls ../private
```
