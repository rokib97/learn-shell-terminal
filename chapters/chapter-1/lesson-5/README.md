# Lesson 5: Shells, REPL, and Variables

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

wagslane@MacBook-Pro ~ % echo hello
hello
wagslane@MacBook-Pro ~ %

In this case:

1. You started with an empty prompt and typed `echo hello`.
2. The shell ran the command and printed the output: `hello`.
3. Finally, the shell gave you a new prompt to type another command: `wagslane@MacBook-Pro ~ %`.

---

## Introduction to Shell Variables

If you're using Ubuntu on WSL, you're probably running a Bash shell.
If you're using macOS, you're probably running a Zsh shell.
If you're running full Linux, I pray you already know what you're using.
The point is that you're probably using Bash or Zsh, and for the purposes of this course, they're basically the same.

Both Bash and Zsh are shells, and they also happen to be powerful programming languages. They have variables, functions, loops, and more. That said, only crazy people write large programs in shell languages... shells are optimized for running other programs and writing small scripts, not for writing large applications.

---

## Create a Variable

To create a variable, you can assign a value like this:

```bash
name="Lane"
```

## Use a Variable

To use the value of a variable, you prefix the variable name with a `$` like so:

```bash
echo $name
# Output: Lane
```

Unlike in Python, where you can just use a variable's name, in your shell, you need to prefix the variable name with a `$` to use it.

---

## Assignment: Forensic Developer Role

For the rest of this course, you'll be a forensic developer hired by the fictional **"WorldBanc"** to investigate a security breach. Like most mega-corporations, they don't know what they're doing, but they're happy to overpay you to come in so that they can say a "third-party expert" has reviewed their systems.

Turns out, you're not an expert, but you're happy to learn on someone else's dime, so why not jump at the opportunity? Right?...

Anyhow, you'll be using your terminal and shell to traverse files, manipulate text, run programs, and investigate suspicious activity.

---

## Set the Following Variables in Your Shell

```bash
bankname="WorldBanc"
founded="1969"
ceo="Jeff Gates"
```

---

## Write a Command That Will Print the Following:

```bash
WorldBanc was founded in 1969 by Jeff Gates
```

### The command that will generate the output is:

```bash
echo $bankname was founded in $founded by $ceo
```

This command will output:

```bash
WorldBanc was founded in 1969 by Jeff Gates
```

---

## Tips

If you're using Windows, certain versions may not let you paste into the Command Line. You can enable `ctrl+shift+v` to paste commands into your terminal.
