# Searching Files with `find`

## What is `find`?

The **`find`** command is a powerful tool for locating files and directories in your system based on their name, size, type, and other attributes. Unlike `grep`, which searches for content inside files, `find` is used to search for files and directories by their names and characteristics.

### Basic Usage

To find a file by its exact name, use the following syntax:

```bash
find directory_path -name "filename"
```

For example, if you're looking for a file named `hello.txt` in your home directory:

```bash
find ~ -name "hello.txt"
```

This will search for `hello.txt` within your home directory.

### Pattern Search

You can use wildcards like `*` to match patterns. For example, to find all `.txt` files:

```bash
find directory_path -name "*.txt"
```

This searches for all files that end with `.txt` in the specified directory.

You can also use `*` to match any part of a filename. For example, if you want to find all files containing "chad" in their name:

```bash
find directory_path -name "*chad*"
```

This will list any files that have "chad" in their name, no matter where the word appears.

## Assignment Instructions

To find files containing the word "joint" in their name within the `worldbanc/public/products` directory, run the following `find` command:

```bash
find worldbanc/public/products -name "*joint*"
```

This will search the `products` directory for files that include the word "joint" in their filename. This can help you investigate accounts that may involve joint owners.

### Helpful Tips

- **Search Subdirectories**: The `find` command searches recursively by default, meaning it will look through all subdirectories inside the specified directory.
- **Case Sensitivity**: By default, `find` is case-sensitive. If you need a case-insensitive search, use the `-iname` option:

  ```bash
  find directory_path -iname "*joint*"
  ```

The `find` command is useful for quickly locating files based on their names or patterns, making it a key tool for file management in the terminal.
