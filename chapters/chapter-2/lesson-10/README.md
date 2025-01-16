# Working with Files in the Terminal: The `mv` Command

## Understanding the `mv` Command

The `mv` command is used to **move** files or directories from one location to another. It can also be used to **rename** files. The `mv` command is essential when you want to reorganize files, change file names, or transfer files between directories.

### Basic Usage:

- **Rename a file:**

  ```bash
  mv old_file.txt new_name.txt
  ```

- **Move a file to a different directory (keeping the same name):**

  ```bash
  mv file.txt target_directory/
  ```

- **Move a file to the parent directory:**

  ```bash
  mv file.txt ../file.txt
  ```

- **Move a file to a specific directory and rename it:**

  ```bash
  mv file.txt target_directory/new_name.txt
  ```

### Why Use `mv`?

- To organize files by moving them to appropriate directories.
- To rename files without creating duplicates.
- To update file locations in the filesystem.

## Assignment Instructions

1. **Navigate to the `credit_cards` Directory:**

   First, make sure you're in the `worldbanc/public/products/credit_cards` directory. You can use the `pwd` command to verify your current location.

   ```bash
   cd worldbanc/public/products/credit_cards
   ```

2. **Move the `tbills.txt` File to the `investments` Directory:**

   The goal is to move `tbills.txt` from the `credit_cards` directory to the newly created `investments` directory. The file should retain its original name.

   Run the following command to move the file:

   ```bash
   mv tbills.txt ../investments/tbills.txt
   ```

3. **Verify the Move:**

   After moving the file, use the `ls` command to list the contents of the `investments` directory and confirm that `tbills.txt` has been moved correctly:

   ```bash
   ls ../investments
   ```

4. **Verify the Directory Structure:**

   Check the contents of the `credit_cards` directory to ensure that `tbills.txt` has been removed, confirming it was successfully moved.

   ```bash
   ls
   ```

## Troubleshooting

- If the file does not move, ensure that both the source and destination paths are correct. Use `pwd` to check your current directory and adjust the paths accordingly.
- If you accidentally move the file to the wrong location, use the `find` command to locate it and move it back to the correct directory.

This guide will help you move files efficiently in the terminal, keeping your filesystem organized and easy to navigate.
