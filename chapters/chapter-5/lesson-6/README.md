# Standard Output

## Overview

Standard output, commonly referred to as stdout, is the default destination where programs send their output. It usually refers to the terminal or console where results are displayed. Standard output can also be redirected to files or other processes for further processing.

## Importance

Understanding how to work with standard output is crucial for logging, debugging, and data extraction. It allows users to interact with program output effectively and automate tasks using command-line tools.

## Common Usage

Standard output is used in various programming languages and command-line utilities to print results. For example:

- In Python:
  ```python
  print("Hello, World!")
  ```
- In Shell:
  ```bash
  echo "Hello, World!"
  ```

## Redirecting Standard Output

Standard output can be redirected to a file using the `>` operator or appended using `>>`.

```bash
echo "Hello" > output.txt
echo "World" >> output.txt
cat output.txt
```

## Example

To find all lines containing the word "Marshal" in a CSV file:

```bash
grep "Marshal" worldbanc/private/transactions/2020.csv
```

### Sample Output:

```
12345,John Marshal,Deposit,5000
67890,Sarah Marshal,Withdrawal,3000
```

## Conclusion

Mastering standard output operations is essential for efficient command-line usage and automation of tasks related to data extraction and manipulation.
