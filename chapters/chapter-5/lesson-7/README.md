# Understanding Standard Error (stderr) and Output Redirection

## What is Standard Error (stderr)?

Standard Error, usually referred to as `stderr`, is a data stream used to output error messages. It functions separately from standard output (`stdout`), allowing users to redirect error messages independently of regular output.

By default, both `stdout` and `stderr` print to the terminal. However, they can be redirected to different locations if necessary.

## Redirecting Streams

You can use redirection operators to send `stdout` and `stderr` to different places:

- `>` redirects `stdout` (standard output)
- `2>` redirects `stderr` (standard error)

### Redirecting stdout to a File

```bash
echo "Hello world" > hello.txt
cat hello.txt
# Output:
# Hello world
```

### Redirecting stderr to a File

```bash
cat doesnotexist.txt 2> error.txt
cat error.txt
# Output:
# cat: doesnotexist.txt: No such file or directory
```

## Assignment Example

There is a script named `process_transactions.sh` located in the `worldbanc/private/bin` directory. This script processes a CSV file and outputs transactions based on the year:

- Modern transactions (after the year 2000) are printed to `stdout`.
- Old transactions (before the year 2000) are printed to `stderr`.

### Steps to Execute the Script

1. Navigate to the appropriate directory or ensure the script path is correct.
2. Run the script by passing the `2020.csv` file located in the `worldbanc/private/transactions` directory.
3. Redirect the stderr output to a temporary log file:

```bash
worldbanc/private/bin/process_transactions.sh worldbanc/private/transactions/2020.csv 2> /tmp/worldbanc.log
```

4. View the redirected stderr output by using the `cat` command:

```bash
cat /tmp/worldbanc.log
```

If the `2020.csv` file is missing, compare the files in the `transactions` directory with those in `transactions/backups` and copy the missing files if necessary:

```bash
cp worldbanc/private/transactions/backups/2020.csv worldbanc/private/transactions/
```

### Key Takeaways

- Use `>` to redirect `stdout` to a file.
- Use `2>` to redirect `stderr` to a file.
- Temporary files in `/tmp` are routinely deleted by the system and are suitable for short-term storage.
