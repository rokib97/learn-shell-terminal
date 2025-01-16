# Viewing Files in the Terminal with `head` and `tail`

## Understanding Files

Files are an essential part of any operating system. They serve as containers for data, whether it’s text, images, or other media. Files can be small or large, and managing them efficiently is key when working with a large amount of data.

## The `head` Command

The `head` command is used to view the first few lines of a file. By default, it shows the first 10 lines, but you can specify a different number of lines if needed.

### Basic Usage:

- **View the first 10 lines of a file:**

  ```bash
  head file1.txt
  ```

- **View the first n lines of a file:**

  ```bash
  head -n 6 file1.txt
  ```

  This will display the first 6 lines of `file1.txt`.

## The `tail` Command

The `tail` command shows the last few lines of a file. Like `head`, it displays 10 lines by default, but you can specify a different number.

### Basic Usage:

- **View the last 10 lines of a file:**

  ```bash
  tail file1.txt
  ```

- **View the last n lines of a file:**

  ```bash
  tail -n 5 file1.txt
  ```

  This will display the last 5 lines of `file1.txt`.

## Assignment Instructions

1. **Navigate to the `worldbanc/private/transactions/` Directory:**

   Use the `cd` command to enter the directory:

   ```bash
   cd worldbanc/private/transactions/
   ```

2. **View the Contents of the `2023.csv` File:**

   Since the file is large, use the `cat` command to inspect the full contents:

   ```bash
   cat 2023.csv
   ```

3. **Use the `head` Command to Print the First 6 Lines:**

   Run the following command to display the first 6 lines, including the header and the first 5 transactions:

   ```bash
   head -n 6 2023.csv
   ```

4. **Use the `tail` Command to Print the Last 5 Lines:**

   Display the last 5 lines of the file:

   ```bash
   tail -n 5 2023.csv
   ```

5. **Combine the First 6 and Last 5 Lines:**

   Copy both the output from the `head` and `tail` commands. You should now have a total of 11 lines to submit.

## Troubleshooting

- If you cannot find the `2023.csv` file, double-check the directory path using the `pwd` command.
- If `head` or `tail` commands aren’t working, ensure you’re in the correct directory and the file exists by running `ls`.

Use this guide to navigate and display portions of large files in the terminal, helping you to work with only the data you need at the moment.
