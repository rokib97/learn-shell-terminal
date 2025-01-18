# Shell Configuration Audit

## Overview

This document guides you through identifying and editing your shell configuration file to determine which commands run automatically upon starting a new shell session.

## Identifying the Active Shell Configuration File

1. **List Hidden Files in the Home Directory:**  
   Run the following command to display hidden files:
   ```bash
   ls -a ~
   ```
2. **Determine Your Shell:**  
   Check your current shell with:
   ```bash
   echo $SHELL
   ```
   - If the output includes `bash`, your configuration file is likely `~/.bashrc`.
   - If it includes `zsh`, your configuration file is likely `~/.zshrc`.

## Editing the Shell Configuration File

1. **Open the Configuration File:**  
   For Bash:

   ```bash
   nano ~/.bashrc
   ```

   For Zsh:

   ```bash
   nano ~/.zshrc
   ```

2. **Add a Test Command:**  
   Scroll to the bottom of the file and add:

   ```bash
   echo "Hello from the shell!"
   ```

3. **Save and Exit:**

   - Press `Ctrl + O` to save the file (confirm with `Enter`).
   - Press `Ctrl + X` to exit the editor.

4. **Verify the Change:**
   - Close the terminal.
   - Open a new terminal session.
   - If you see the message `Hello from the shell!`, the correct configuration file was edited.

## Cleanup

1. **Remove the Test Command:**  
   Reopen the configuration file:

   ```bash
   nano ~/.bashrc   # For Bash
   nano ~/.zshrc    # For Zsh
   ```

2. **Delete the Line:**  
   Remove:

   ```bash
   echo "Hello from the shell!"
   ```

3. **Save and Exit:**
   - Press `Ctrl + O` to save.
   - Press `Ctrl + X` to exit.
