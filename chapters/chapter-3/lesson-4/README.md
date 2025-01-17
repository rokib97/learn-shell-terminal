## Executables

Executable files are files where the data stored inside is a program that you can run on your computer. A common example is a shell script, which is a file containing shell commands.

### Running Shell Scripts

To run a shell script, you need to specify its filepath. If the script is in the current directory, you need to prefix it with `./` to execute it.

Example:

```
./program.sh
```

### Assignment: Modifying Permissions

There seems to be a suspicious script in the `worldbanc/private/bin` directory called `genids.sh`. It likely generates some kind of identifier.

The task is to remove our ability to run this script by adjusting its file permissions.

#### Steps:

1. **Remove Execute Permission:**
   In the `worldbanc/private/bin` directory, run the following command to remove the executable permission from `genids.sh`:

   ```
   chmod -x genids.sh
   ```

2. **Test the Permission Change:**
   Try running the script with:

   ```
   ./genids.sh
   ```

   You should get an error like:

   ```
   permission denied
   ```

3. **Re-add Execute Permission:**
   To restore the ability to run the script, add the executable permission back for the owner:

   ```
   chmod +x genids.sh
   ```

4. **Test Again:**
   Once you've added the execute permission, run the script again with:
   ```
   ./genids.sh
   ```
