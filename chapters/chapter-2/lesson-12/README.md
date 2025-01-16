## Copy Command

The `cp` command allows you to copy a file or directory from one location to another.

### Copy a file

To copy a file, use the following command:

```bash
cp source_file.txt destination/
```

### Copy a directory recursively

You can also copy a directory and all of its contents recursively by adding the `-R` flag:

```bash
cp -R my_dir new_dir
```

---

## Assignment: Verifying Transaction Backups

1. Navigate to the `worldbanc/private/transactions/` directory.

   - You should see several files containing transaction data from different years.

2. Inside the `transactions` directory, locate the `backups` folder. It seems that something is missing!

3. Copy the missing file from the `transactions` directory into the `backups` directory so that all transactions have a backup.

4. Once you've copied the file, list the contents of the `backups` directory to verify the backup.

```bash
ls backups/
```

5. **Verification**: Ensure that the missing file now appears in the `backups` directory. If the file is correctly copied, the backup is successfully completed.
