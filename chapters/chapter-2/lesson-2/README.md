# WorldBanc Setup Guide

## Understanding Filepaths

A **filepath** is a string that describes the location of a file or directory on your computer. An example of a filepath looks like this:

```
/Users/wagslane
```

### Breakdown of the Filepath:

- **/** : Represents the **root directory**, the topmost level of the filesystem.
- **Users** : A directory inside the root directory.
- **wagslane** : A directory inside the Users directory.

This structure represents a path two levels down from the root directory:

```
root
└── Users
    └── wagslane
```

---

## Assignment: Download and Set Up the WorldBanc Directory

### Step 1: Download the WorldBanc Directory

Run the following commands in your terminal to download and set up the **worldbanc** directory from the provided GitHub repository:

```bash
# Clone the worldbanc directory from GitHub
git clone https://github.com/rokib97/learn-shell-terminal.git

# Navigate to the worldbanc folder
cd learn-shell-terminal/worldbanc
```

### Step 2: Verify the Setup

1. **List Directory Contents**  
   Run the following command to verify the **worldbanc** directory exists:

   ```bash
   ls
   ```

   You should see various files and folders inside the `worldbanc` directory.

2. **Navigate into the worldbanc Directory**  
   Ensure you are inside the correct directory:

   ```bash
   pwd
   ```

   The output should confirm the correct path: `.../learn-shell-terminal/worldbanc`

3. **List Contents of worldbanc**  
   Verify its contents:

   ```bash
   ls
   ```

---

## Troubleshooting

- **git not installed?**  
  Install it using:

  ```bash
  sudo apt install git
  ```

- **Can't paste in the terminal?**  
  Use **Ctrl + Shift + V** to paste commands.

If any issues occur, revisit the steps to redownload and set up the directory.
