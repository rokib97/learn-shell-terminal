# Piping in the Shell

Piping is a powerful feature in the shell that allows you to send the output of one command directly into the input of another. This enables complex automation tasks to be accomplished efficiently.

## What is Piping?

The **pipe operator** (`|`) allows you to take the **stdout** (output) of one command and send it as the **stdin** (input) to another command. This makes it possible to chain multiple commands together in a single line to perform advanced tasks.

### Example: Basic Pipe Usage

Let’s consider the following example:

```bash
echo "Have you heard the tragedy of Darth Plagueis the Wise?" | wc -w
```

- The `echo` command outputs the text `"Have you heard the tragedy of Darth Plagueis the Wise?"`.
- The pipe operator (`|`) sends the output from `echo` as input to the `wc` command.
- The `wc` command counts the number of words in the input received. The `-w` flag tells `wc` to count only words.

The result is:

```
10
```

## Assignment: Count Transactions Involving "Bob"

Let’s use piping to count how many transactions involve "Bob" in a directory of transaction files.

### Step 1: Search for Transactions Involving "Bob"

To search for the word "Bob" in all files within the `worldbanc/private/transactions` directory, but **excluding** the `backups` directory, use the following command:

```bash
grep -R "Bob" worldbanc/private/transactions --exclude-dir="backups"
```

- `grep -R "Bob"` searches recursively for the word "Bob" in all files.
- `--exclude-dir="backups"` ensures that files in the `backups` directory are excluded from the search.

### Step 2: Count the Number of Transactions

To count the number of occurrences (lines) involving "Bob," pipe the output of the `grep` command into `wc -l`:

```bash
grep -R "Bob" worldbanc/private/transactions --exclude-dir="backups" | wc -l
```

This will output the total number of transactions involving "Bob."

### Final Step: Submit the Result

- Copy the **number of transactions** from the output (just the number itself).
- Paste it into the provided text field and submit your answer.

## Tip

If your result is incorrect (e.g., if you get 3002 transactions), make sure that the files in the `transactions` directory match the files in `transactions/backups`. If they don't, create a copy of the correct files.
