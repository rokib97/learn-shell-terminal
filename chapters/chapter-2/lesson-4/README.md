# Absolute vs. Relative Paths

## Understanding File Paths

File paths are used to locate files and directories within a filesystem. They can be **absolute** or **relative**, depending on how they reference locations.

---

## Relative Paths

A **relative path** specifies a file or directory location based on the current working directory.

### Example Directory Structure:

```
vehicles
├── cars
│   ├── fords
│   │   ├── mustang.txt
│   │   └── focus.txt
```

### Relative Path Examples:

- From the `vehicles` directory to `mustang.txt`:
  ```bash
  cars/fords/mustang.txt
  ```
- From the `cars` directory to `mustang.txt`:
  ```bash
  fords/mustang.txt
  ```
- From the `fords` directory to `mustang.txt`:
  ```bash
  mustang.txt
  ```

Relative paths are shorter and easier to work with when you're in or near the target directory.

---

## Absolute Paths

An **absolute path** specifies a file or directory location starting from the root directory `/`.

### Absolute Path Example:

If `vehicles` is located at the root of the filesystem, the absolute path to `mustang.txt` is:

```bash
/vehicles/cars/fords/mustang.txt
```

Regardless of the current directory, this path always points to the same file.

---

## Choosing Between Absolute and Relative Paths

### When to Use Relative Paths:

- When working within a known directory structure.
- For shorter and more readable commands.
- In scripts that are run from specific directories.

### When to Use Absolute Paths:

- When the current directory may vary.
- When providing exact file locations to others.
- In scripts that must work regardless of the working directory.

---

## Summary

- **Relative Path:** Depends on the current directory. Easier for internal navigation.
- **Absolute Path:** Starts from the root `/`. More reliable for universal access.

Using the appropriate path type improves workflow efficiency and reduces navigation errors.
