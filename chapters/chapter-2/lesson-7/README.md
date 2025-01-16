# Viewing Files in the Terminal with `more` and `less`

## Understanding File Browsing

When working with large files in the terminal, it’s often impractical to view everything at once. The `more` and `less` commands allow you to view file contents one page at a time. These commands provide an interactive experience, making it easier to navigate large files.

### The `more` Command

The `more` command is used to view the contents of a file one screen at a time. It’s a basic pager that allows you to scroll down a file, but it doesn't have as many features as the `less` command.

### The `less` Command

The `less` command is a more advanced pager that allows you to scroll both forward and backward through a file. It also includes additional features, such as line numbers, making it more versatile than `more`. It is recommended to use `less` instead of `more` when available.

### Basic Usage:

- **View the file content one page at a time:**

  ```bash
  less filename.txt
  ```

- **Scroll down by pressing `Enter` to move one line at a time.**

- **Scroll down by pressing the spacebar to move a full page.**

- **Scroll up by pressing `b` (back).**

- **Exit the `less` program by pressing `q`.**

## Assignment Instructions

1. **Run the `less` Command on the `2023.csv` File:**

   Navigate to the `worldbanc/private/transactions/` directory and run the following command:

   ```bash
   less 2023.csv
   ```

   You’ll be taken into an interactive mode where you can scroll through the file one page at a time. Press `Enter` to scroll down one line, or press the spacebar to move a full page down. Press `q` to exit when you’re done.

2. **Use the `-N` Flag to Display Line Numbers:**

   Run the following command to see the line numbers along with the content of the file:

   ```bash
   less -N 2023.csv
   ```

   This will allow you to keep track of the exact line number you're viewing. Use the spacebar to scroll down or press `b` to go back.

3. **Find and View Line 153:**

   Scroll through the file or use the line number to navigate directly to line 153. You can do this by searching for the line number or manually scrolling until you reach it.

4. **Verify the Content of Line 153:**

   After navigating to line 153, verify the content displayed. Ensure that it’s the correct line and matches the expected data.

5. **Exit the `less` Program:**

   Once you've completed the verification, press `q` to exit `less` and return to the terminal prompt.

## Troubleshooting

- If `less` doesn’t work, it might not be installed on your system. In that case, you can use `more`, but `less` is recommended when available.
- Use the `q` key to exit the `less` program if you feel stuck.

This guide will help you navigate large files more effectively, allowing you to examine specific sections of the file without printing everything to the terminal.
