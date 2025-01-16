# Understanding the Filesystem

## What Is a Filesystem?

All the data stored on your computer is organized into **files** and **directories**. These files and directories are structured in a hierarchical, tree-like format known as a **filesystem**.

### Key Concepts:

- **Directories (Folders):** Containers that hold files and other directories.
- **Files:** Collections of raw binary data (1's and 0's) that can represent text, images, videos, programs, etc.
- **Root Directory (/):** The starting point of the filesystem. All files and directories branch out from here.

### Filesystem Structure Example:

```
/
├── home
│   ├── user
│   │   ├── documents
│   │   └── downloads
├── etc
├── var
└── usr
```

- The `/` represents the root directory.
- `/home/user` is a user's home directory where personal files are typically stored.

### Working Directory

When you open a terminal, you're placed in a **working directory**. This is commonly your **home** directory, but it can vary depending on the system or session.

## Assignment

You've remotely accessed a suspicious employee's computer at **WorldBanc**. Your first task is to determine your current location in the filesystem.

### Step 1: Print the Current Working Directory

Run the following command in the terminal to verify your current directory:

```bash
pwd
```

**Example Output:**

```
/home/worldbanc_employee
```

If the output shows a directory path, you've successfully verified your current working directory.
