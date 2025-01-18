### 1. **What is the PATH Variable?**

The `PATH` environment variable contains a list of directories. When you run a command in the terminal, the shell searches these directories to find an executable file that matches the command. If the executable is found, it runs the command; otherwise, you get an error.

For example, if you type `ls`, your shell searches the directories listed in your `PATH` to find the `ls` executable. Common directories might include `/bin`, `/usr/bin`, and `/usr/local/bin`.

#### Why Do We Care About PATH?

Without `PATH`, you would have to type out the full path to any executable every time. For instance, instead of just typing `ls`, you would have to type `/bin/ls` or wherever the `ls` command is located. This is cumbersome and inefficient.

### 2. **What’s Inside the PATH Variable?**

To see your current `PATH` variable, you can use the following command:

```bash
echo $PATH
```

This will display a list of directories separated by colons (`:`). Each directory in the list is a place the shell checks for executables.

For example, if the output is:

```
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
```

Your shell will look for executables in these directories, in order, whenever you run a command.

### 3. **Assignment 1: Temporarily Disable the PATH**

To temporarily disable the `PATH`, run:

```bash
export PATH=""
```

This clears the `PATH` for the current shell session. As a result, your shell won't be able to find any executables unless you provide their full path.

Now, try running some commands like `ls`, `pwd`, `echo`. Some will fail because they rely on the directories in your `PATH`. For example:

```bash
$ ls
-bash: ls: command not found
```

This is because `ls` is located in `/bin/`, which is no longer part of your `PATH`.

### 4. **Assignment 2: Add a Directory to the PATH**

When you install a program, it often installs executables in a directory not in your `PATH`. To run these programs without specifying their full path, you need to add their directory to your `PATH`.

Let's say you have a directory with useful executables (`worldbanc/private/bin`), and you want to add it to your `PATH`.

#### Steps to Add a Directory to PATH:

1. **Get the Absolute Path:**
   Navigate to the `worldbanc/private/bin` directory:

   ```bash
   cd /path/to/worldbanc/private/bin
   ```

   Then, get the absolute path of this directory:

   ```bash
   pwd
   ```

   This will print the absolute path, for example:

   ```
   /home/user/worldbanc/private/bin
   ```

2. **Add to PATH:**
   To add the new directory to your `PATH` without removing the existing directories, use the following command:

   ```bash
   export PATH="$PATH:/home/user/worldbanc/private/bin"
   ```

   This appends the directory to your current `PATH`. Now, the shell will look for executables in `/home/user/worldbanc/private/bin` as well.

3. **Check if It Works:**
   To verify that the directory was added successfully, run:

   ```bash
   echo $PATH
   ```

   You should now see `/home/user/worldbanc/private/bin` listed as part of your `PATH`.

4. **Run the Script:**
   Now that the directory is in your `PATH`, you can run the `worldbanc.sh` shell script from anywhere:

   ```bash
   worldbanc.sh
   ```

   Since `worldbanc.sh` is in the `/home/user/worldbanc/private/bin` directory (which is now part of your `PATH`), the shell can find and execute it.

### 5. **Reset the PATH to Default**

After the changes, if you want to revert your `PATH` to its default settings, close the terminal window and open a new one. This will reset the `PATH` to its default state.

Alternatively, if you want to permanently modify your `PATH` (for example, for future sessions), you can add the `export PATH` line to your shell's profile file (`~/.bashrc`, `~/.zshrc`, etc.).

### Key Takeaways:

- The `PATH` variable is essential for running executables without typing the full path.
- Modifying the `PATH` allows you to run commands from new directories without needing their full paths.
- Disabling the `PATH` temporarily can prevent unintended executions but is impractical for regular use.
- Adding directories to the `PATH` makes executables from those directories accessible from anywhere.
