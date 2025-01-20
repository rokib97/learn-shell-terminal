# Working with Directories in the Terminal: The `mkdir` Command

## Understanding Directories

A **directory** (sometimes called a "folder") is a container used to store files and other directories. It helps in organizing files in a hierarchical structure, making it easier to navigate through the filesystem.

### The `mkdir` Command

The `mkdir` command stands for "make directory" and is used to create new directories within the current directory.

### Basic Usage:

- **Create a new directory:**

  ```bash
  mkdir my_directory
  ```

- **Create multiple directories at once:**

  ```bash
  mkdir dir1 dir2 dir3
  ```

### Why Use `mkdir`?

- To organize files into specific folders.
- To create new directories for projects or different categories of files.
- To keep the filesystem clean and easy to navigate.

## Assignment Instructions

1. **Navigate to the `credit_cards` Directory:**

   Make sure you're in the `worldbanc/public/products/credit_cards` directory:

   ```bash
   cd worldbanc/public/products/credit_cards
   ```

2. **List the Contents of the `credit_cards` Directory:**

   Run the `ls` command to view the contents of the directory. You should see a file named `tbills.txt`. This file doesn’t belong in the `credit_cards` directory because it is related to investments, not credit cards.

   ```bash
   ls
   ```

3. **Go Back to the `products` Directory:**

   Navigate back to the `worldbanc/public/products` directory:

   ```bash
   cd ..
   ```

4. **Create the `investments` Directory:**

   Run the following command to create a new directory named `investments` in the `products` directory:

   ```bash
   mkdir investments
   ```

5. **Verify the Directory Creation:**

   After creating the `investments` directory, use the `ls` command to confirm that the new directory is present in the `products` directory:

   ```bash
   ls
   ```

6. **Verify the Contents:**

   Once you've confirmed the creation of the `investments` directory, check if the file `tbills.txt` is out of place in the `credit_cards` directory and ensure the directory structure is as expected.

## Troubleshooting

- If you cannot create a directory, check if you have permission to write to the parent directory. Use `ls -l` to check the permissions of the current directory.
- If you’re unsure about your current location, use the `pwd` command to verify the path.

This guide helps you manage and organize files into directories, providing a structured way to keep your project files organized.
