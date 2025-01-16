# Lesson 4: What Is a Shell?

## Understanding the Shell

A **shell** is a program that interprets and executes the commands you type into a terminal. It allows you to interact with the operating system by issuing text-based commands and receiving the results of those commands.

### Main Role of a Shell

- **Interpretation:** The shell reads the command you type and determines how to execute it.
- **Execution:** The shell runs the command by launching other programs or processes on your computer.
- **Output:** The shell displays the results of the executed command and then returns control to you with a new prompt.

### Shells as REPLs

Shells are often referred to as **REPLs**, which stands for:

- **Read**: The shell reads the command you input.
- **Eval (Evaluate)**: The shell processes and evaluates the command.
- **Print**: The shell displays the output.
- **Loop**: The shell provides a new prompt, ready for the next command.

### Example Shell Output

When you type a command in a shell, the process looks like this:

```bash
$ expr 123456 + 7890
131346
$
You enter expr 123456 + 7890.
The shell runs the expr program, evaluates the sum, and prints the result 131346.
It then gives you a new prompt ($) to type the next command.
Assignment
In your shell, run the following command:

bash
Copy
Edit
expr 123456 + 7890
Paste the output of that command into the text box on the right.

Tip
To help clarify the difference between prompts and outputs, here's a quick breakdown:

Prompt: The shell’s request for a command, usually in the format $ or username@hostname ~ %.
Output: The result produced by the command, displayed after you execute it.
```
