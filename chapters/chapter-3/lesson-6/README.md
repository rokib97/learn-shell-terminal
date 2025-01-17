## Chown - Change Ownership

The `chown` command is used to change the ownership of a file or directory. If you don’t own a file or directory, you’ll need `sudo` (root privileges) to change its ownership.

### When to Use `sudo` with `chown`

While `chmod` allows you to change the permissions of any file or directory that you own, `chown` allows you to change the owner of a file or directory. Since this command affects ownership, it requires root privileges.

### Assignment: Changing Ownership of a Directory

In this assignment, we will change the owner of a directory to `root` using `chown`. Here are the steps:

1. **Navigate to the Directory**:
   Change into the `worldbanc/private` directory:

   ```
   cd worldbanc/private
   ```

2. **List the Contents**:
   Take a look at the contents with the `ls` command:

   ```
   ls
   ```

   You should see a directory called `contacts`.

3. **Inspect the Contents of the `contacts` Directory**:
   Change into the `contacts` directory:

   ```
   cd contacts
   ```

   List its contents:

   ```
   ls
   ```

   You should see a file called `emergency.txt`.

4. **View the Contents of the File**:
   Display the contents of `emergency.txt` with the `cat` command:

   ```
   cat emergency.txt
   ```

   This file contains personal contact information, and we want to limit its access.

5. **Change Ownership**:
   Change the owner of the entire `contacts` directory to `root` using the following command:

   ```
   sudo chown -R root contacts
   ```

   - `sudo`: Run the command as the root user
   - `chown`: Command to change the owner
   - `-R`: Apply the changes recursively to everything inside the directory
   - `root`: The new owner
   - `contacts`: The directory to change ownership of

6. **Verify Ownership Change**:
   From the `worldbanc/private` directory, run the following command to check the ownership:
   ```
   ls -l
   ```
