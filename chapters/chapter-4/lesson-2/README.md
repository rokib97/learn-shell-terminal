## Shebang (#!)

A **shebang** is a special line at the top of a script that tells the system which interpreter to use to run the script.

### Format

```bash
#! interpreter [optional-arg]
```

### Example

For a Python script using Python 3:

```bash
#!/usr/bin/python3
```

This instructs the system to use the Python 3 interpreter located at `/usr/bin/python3`.

### Viewing a Shebang

To view the shebang of a script, use the `cat` command:

```bash
cat private/bin/genids.sh
```

This command displays the shebang line at the top of the script, verifying which interpreter will run the script.
