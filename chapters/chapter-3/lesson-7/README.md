## Using `sudo` to Delete a Directory

Before starting this assignment, ensure that the permissions on the `worldbanc/private/contacts` directory are set to `drwx------`, the owner is `root`, and you're not signed in as the `root` user. You can check these with the `ls -l` command.

### Assignment: Deleting the `contacts` Directory

In this assignment, you'll delete the `contacts` directory. Since the directory is owned by `root`, you will need to use `sudo` to perform the action.

#### Steps:

1. **Check the Permissions and Ownership**:
   Before proceeding, verify that the `contacts` directory has the correct permissions and ownership:

   ```
   ls -l worldbanc/private/contacts
   ```

   The directory should be `drwx------`, and the owner should be `root`.

2. **Try Deleting the Directory Without `sudo`**:
   Attempt to delete the `contacts` directory using the `rm` command:

   ```
   rm -r contacts
   ```

   Since you don’t have permission to delete it (the owner is `root`), the command should fail.

3. **Delete the Directory with `sudo`**:
   To delete the directory, use `sudo` to run the command as the root user:

   ```
   sudo rm -r contacts
   ```

   This will allow you to delete the directory since `sudo` gives you the necessary elevated privileges.

4. **Verify Deletion**:
   Once the directory is deleted, run the following command from inside the `worldbanc/private` directory:
   ```
   ls
   ```
   This will list the remaining contents of the `private` directory.
