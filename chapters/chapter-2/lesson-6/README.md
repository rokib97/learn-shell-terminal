# Lesson 6: Shell Command History

## Viewing Command History

When you're working in a REPL, it's really helpful to be able to see the commands you've typed in the past. This makes it easier to:

- Re-run previous commands
- Copy and paste commands into a script for reuse

To print out the history of commands you've typed in your shell, you can use the `history` command:

```bash
history
```

This will display a list of all previously executed commands in your current shell session.

---

## Assignment

### Step 1: Set Variables

In your shell, set two variables:

```bash
department="engineering"
team="ops"
```

### Step 2: Print a Message Using Variables

Use the `echo` command to print the following message by referencing the variables:

```bash
echo "I work in $department on $team"
```

**Expected Output:**

```
I work in engineering on ops
```

### Step 3: View Command History

Run the `history` command to view the list of previously executed commands:

```bash
history
```

This will display the sequence of commands you've used, including the variable assignments and the `echo` command.

---

## Example Output

```bash
1  department="engineering"
2  team="ops"
3  echo "I work in $department on $team"
4  history
```

This output shows the steps taken to complete the assignment and how the `history` command lists those actions.
