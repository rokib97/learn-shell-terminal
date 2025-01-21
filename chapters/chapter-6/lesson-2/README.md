# Editing a File Using Neovim

## Assignment Overview

A public file contains a company password that needs to be redacted. This guide will walk you through editing the file using Neovim and replacing the sensitive information.

---

## Steps to Edit and Save the File

### 1. Open the File

To open the target file, run the following command in your terminal:

```bash
nvim worldbanc/public/company_info.md
```

This will open the Markdown file in Neovim.

---

### 2. Navigate to the Password

- Upon opening, you'll be in **normal mode**, which is used for navigating and manipulating text.
- Use the **arrow keys** to move the cursor to the last line where the password is located.

---

### 3. Enter Insert Mode

Once you've positioned the cursor correctly:

- Press `i` to enter **insert mode** (you should see `-- INSERT --` at the bottom of the screen).
- Delete the password and replace it with:

  ```text
  REDACTED
  ```

---

### 4. Save the Changes

After replacing the password:

- Press `esc` to return to **normal mode**.
- Type `:w` and press **Enter** to save the changes.

---

### 5. Exit Neovim

Once the changes are saved:

- Type `:q` and press **Enter** to quit Neovim.

---

### 6. Verify the Changes

To confirm the file was edited correctly, use the following command:

```bash
cat worldbanc/public/company_info.md
```

This will display the updated contents of the file in the terminal.

---

### Conclusion

Congratulations! You've successfully:

- Opened the file in Neovim
- Navigated and edited the content
- Saved and exited without issues
- Verified the changes using `cat`

Mastering these basic Neovim commands is an essential skill for developers.
