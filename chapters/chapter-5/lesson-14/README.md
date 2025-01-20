# Searching Files with `grep`

## What is `grep`?

The **`grep`** command is a powerful tool used in the terminal to search for specific text or patterns in files. It's commonly used for finding keywords or phrases in logs, scripts, and other text files.

### Basic Usage

To search for a word or phrase in a file using `grep`, you can run the following command:

```bash
grep "search_term" filename
```

For example, if you want to find the word "hello" in a file called `words.txt`, you would use:

```bash
grep "hello" words.txt
```

This will display all lines in `words.txt` that contain the word "hello". It’s case-sensitive, meaning it will only match exactly "hello" (not "Hello" or "HELLO").

## Searching Multiple Files

You can search for a term in more than one file at a time by specifying multiple filenames:

```bash
grep "search_term" file1.txt file2.txt
```

This will show matches for the term in both `file1.txt` and `file2.txt`.

## Recursive Search

If you want to search for a term in an entire directory, including all subdirectories, you can use the `-r` (recursive) flag:

```bash
grep -r "search_term" .
```

Here, the `.` represents the current directory. This command will search through all files in the current directory and any subdirectories.

## Assignment Instructions

1. **Search for "CRITICAL" in a Log File:**

   Use the `grep` command to search for the word "CRITICAL" (in all caps) in the file located at:

   ```bash
   worldbanc/private/logs/2024-01-10.log
   ```

   The command would look like this:

   ```bash
   grep "CRITICAL" worldbanc/private/logs/2024-01-10.log
   ```

2. **Search for "CRITICAL" in the Entire Logs Directory:**

   To search for the word "CRITICAL" across all files in the `logs` directory, including any subdirectories, use the recursive flag:

   ```bash
   grep -r "CRITICAL" worldbanc/private/logs
   ```

   This will search through all the files in `logs` and display any lines containing "CRITICAL".

### Helpful Tips

- **Autocompletion**: When typing a file or directory name, press **Tab** to autocomplete it.
- **Case Sensitivity**: The search is case-sensitive by default. If you need a case-insensitive search, use the `-i` flag:

  ```bash
  grep -i "critical" filename
  ```

By using `grep`, you can quickly and efficiently search through files and logs for specific information.
