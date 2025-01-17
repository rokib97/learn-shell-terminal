## Changing Permissions

The `chmod` command is used to change file and directory permissions. It stands for **change mode**.

### Syntax

```
chmod [options] permissions file/directory
```

### Assignment: Secure the Private Directory

1. **Check Current Permissions:**  
   Use the `ls -l` command to display the permissions of the files in the `worldbanc/private` directory:

   ```bash
   ls -l worldbanc/private
   ```

2. **Update Permissions:**  
   Modify the permissions of the `private` directory and all its contents so that:

   - **Owner** can **read**, **write**, and **execute**
   - **Group** has **no permissions**
   - **Others** have **no permissions**

   Run the command:

   ```bash
   chmod -R u=rwx,g=,o= worldbanc/private
   ```

3. **Verify Permissions:**  
   Run the `ls -l` command again to ensure the permissions have been updated:

   ```bash
   ls -l worldbanc/private
   ```

4. **Automatic Verification:**  
    The system will automatically verify if the permissions for the `private` directory are set to `drwx------`.

   **Expected Output:**

   ```
   drwx------ 2 user group 4096 Jan 17 10:00 private
   ```

---

⚠️ **Note:** Be cautious when using `chmod` with the `-R` flag as it recursively changes permissions for all contents in the directory.
