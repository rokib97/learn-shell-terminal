# Understanding Standard Input (stdin)

## Overview

Standard Input, commonly referred to as **stdin**, is the default data stream that programs use to receive input from the user or another source. In most operating systems, stdin is typically connected to the keyboard, allowing users to input data interactively.

## How stdin Works

When a program runs and requires input, it will pause execution and wait for data from stdin. Once the user provides input and presses **Enter**, the program processes the provided data.

## Reading from stdin in Different Programming Languages

- **Bash (Shell Scripting):**

  ```bash
  read -p "Enter your name: " name
  echo "Hello, $name"
  ```

- **Python:**
  ```python
  # execution stops until the user types
  # something (in this case "Lane") and presses enter
  name = input("What is your name? ")
  print("Hello,", name)
  # Hello, Lane!
  ```

**Sample Interaction:**

```
What is your name? Lane
Hello, Lane
```

## Redirecting stdin

stdin can also be redirected from files or other streams using operators like `<` in command-line environments.

Example:

```bash
python script.py < input.txt
```

This feeds the content of `input.txt` to `script.py` as stdin input.

## Assignment

Run the `worldbanc/private/bin/worldbanc.sh` program again. Notice that it makes use of stdin to read your name and email.

Take a closer look at the code in the `worldbanc.sh` file. What command does it use to read from stdin?

## Conclusion

Understanding and using stdin effectively allows for dynamic user input handling and automation through redirection. Most programming languages provide built-in ways to read from stdin, making it a fundamental concept in software development.
