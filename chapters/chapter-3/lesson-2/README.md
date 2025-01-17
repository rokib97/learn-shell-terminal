# File and Directory Permissions

## Understanding Permissions

In Unix-like operating systems, permissions define who can read, write, or execute files and directories. These permissions are represented by a 10-character string:

```
drwxrwxrwx
```

### Breakdown of Permissions

1. **File Type** (First Character)

   - `-` → Regular file (e.g., `-rwxrwxrwx`)
   - `d` → Directory (e.g., `drwxrwxrwx`)

2. **Permission Groups** (Next few Characters)  
   Split into three sets of `rwx` for:

   - **Owner** (User)
   - **Group**
   - **Others**

   | Symbol | Permission | Action              |
   | ------ | ---------- | ------------------- |
   | `r`    | Read       | View file contents  |
   | `w`    | Write      | Modify the file     |
   | `x`    | Execute    | Run the file/script |

### Examples

- `-rwxrwxrwx`: A file where everyone can read, write, and execute.
- `-rwxr-xr-x`: A file where everyone can read and execute, but only the owner can write.
- `drwxr-xr-x`: A directory where everyone can view and enter, but only the owner can modify it.
- `drwx------`: A directory only accessible by the owner.
