# Navigating Parent Directories in the Filesystem

## Understanding Parent Directories

In the filesystem, directories are organized in a hierarchical structure. The **`cd`** command is used to navigate into directories, but to move back up to a parent directory, you can use the special alias:

```bash
..
```

### Key Concept:

- **`..`** refers to the **parent directory** of your current working directory.
- This allows you to move **up one level** in the directory tree.

### Example:

If you're currently in:

```
/home/user/worldbanc
```

Running:

```bash
cd ..
```

Will take you to:

```
/home/user
```

## Assignment

### Step 1: Navigate to the Parent Directory

If you're inside the **worldbanc** directory, move up to its parent directory using:

```bash
cd ..
```

### Step 2: List the Contents of the worldbanc Directory

From the parent directory, list the contents of the **worldbanc** directory with:

```bash
ls worldbanc
```

### Example Output:

```
README.md
logs
scripts
config
```

This command displays the contents of the **worldbanc** directory without needing to navigate back into it.

## Notes

- **`cd ..`** moves you up one level in the directory hierarchy.
- **`ls [directory]`** lists the contents of a directory without changing your current location.

Use these commands to efficiently navigate and explore directories in your filesystem.
