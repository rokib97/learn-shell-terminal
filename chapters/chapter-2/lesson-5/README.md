# Viewing Files in the Terminal

## Understanding Files

Files are fundamental components of any operating system. They are essentially blobs of data where the raw bytes can represent anything—text, images, videos, and more.

## The `cat` Command

The `cat` command, short for **concatenate**, is primarily used to display the contents of files in the terminal. While it may seem unintuitive for viewing single files, its true power lies in combining and displaying multiple files at once.

### Basic Usage:

- **View the contents of a single file:**

  ```bash
  cat file1.txt
  ```

- **Concatenate and view multiple files:**

  ```bash
  cat file1.txt file2.txt
  ```

## Assignment Instructions

1. **Navigate to the `worldbanc` Directory:**

   If you're not already in the `worldbanc` directory, run:

   ```bash
   cd worldbanc
   ```

2. **Confirm Your Location:**

   Use the `ls` command to verify that you're in the correct directory. You should see a `public` directory listed:

   ```bash
   ls
   ```

3. **Access the `public` Directory:**

   Change into the `public` directory:

   ```bash
   cd public
   ```

4. **Locate the `pr_ideas.txt` File:**

   Confirm that the `pr_ideas.txt` file is present:

   ```bash
   ls
   ```

5. **View the Contents of `pr_ideas.txt`:**

   Display the file's contents using the `cat` command:

   ```bash
   cat pr_ideas.txt
   ```

If you successfully see the contents of `pr_ideas.txt`, you've completed this task!

## Troubleshooting

- If you cannot find the `public` directory, ensure you're in the correct location by running `pwd`.
- If `cat` isn't working, make sure the file exists by running `ls` first.

Use this guide to effectively navigate and read files in the terminal.
