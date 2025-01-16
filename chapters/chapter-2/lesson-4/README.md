# Lesson 4: Understanding Shells and REPL

## What Is a Shell?

The terminal is a program that allows you to issue text-based commands and view the output of those commands. But what is the program that runs those commands? That's a shell.

Shells do a lot of things, but their main job is to interpret the commands you type and execute them.

## Shells as REPL

Shells are often referred to as "REPL"s, which stands for:

- **Read**: The shell reads the command you type.
- **Eval (Evaluate)**: The shell evaluates the command by running other programs on your computer.
- **Print**: The shell prints the output of the command.
- **Loop**: The shell gives you a new prompt to type another command and repeats the process.

In simple terms, shells:

1. Read the commands you type.
2. Evaluate those commands by running the corresponding programs.
3. Print the output of the commands.
4. Give you a new prompt to type another command and continue the loop.

---

## Example Command Output

For example, in the terminal:

```bash
wagslane@MacBook-Pro ~ % echo hello
hello
wagslane@MacBook-Pro ~ %
```
