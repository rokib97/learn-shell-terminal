# Compiled vs. Interpreted Programs

## Overview

A program is a set of instructions that a computer can execute. These programs can be categorized broadly into two types:

- **Compiled Programs**
- **Interpreted Programs**

## Compiled Programs

A compiled program is transformed from human-readable source code into machine code (binary) through a compiler. The resulting executable file can run directly on a computer's CPU without needing any additional software.

### Characteristics

- **Languages:** Go, C, Rust
- **Execution:** Directly by the CPU
- **Performance:** Typically faster due to direct execution
- **Distribution:** Can be shared as standalone executables

## Interpreted Programs

An interpreted program is executed by another program called an interpreter. The interpreter reads and executes the source code line-by-line or block-by-block.

### Characteristics

- **Languages:** Python, Ruby, JavaScript
- **Execution:** Requires an interpreter (e.g., Python interpreter, Node.js for JavaScript)
- **Performance:** Slower due to real-time interpretation
- **Distribution:** Source code is shared and run through interpreters

### Example

- `.sh` files (shell scripts) are interpreted by the shell program (e.g., `sh`).

## Practical Example

1. **Find the location of the `sh` program:**
   ```bash
   which sh
   ```
   Example Output:
   ```
   /bin/sh
   ```
2. **View the contents of the `sh` program:**

   ```bash
   cat /bin/sh
   ```

   Output will be unreadable because `/bin/sh` is a compiled binary.

3. **View a shell script:**
   ```bash
   cat script.sh
   ```
   Output will be readable because `.sh` files are text-based commands interpreted by `sh`.

## Key Differences

| Feature             | Compiled Programs          | Interpreted Programs     |
| ------------------- | -------------------------- | ------------------------ |
| **Translation**     | Compiled into machine code | Interpreted at runtime   |
| **Execution Speed** | Faster                     | Slower                   |
| **Portability**     | Platform-dependent         | More portable            |
| **Error Detection** | At compile-time            | At runtime               |
| **Examples**        | Go, C, Rust                | Python, Ruby, JavaScript |

## Conclusion

Both compiled and interpreted programs serve specific use cases. Compiled languages are preferred for performance-critical applications, while interpreted languages offer flexibility and ease of development.
