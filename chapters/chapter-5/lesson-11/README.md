# Killing a Malicious Process

## Overview

This guide will help you safely terminate a malicious program that does not respond to the usual `CTRL+C` command by manually identifying its process ID (PID) and using the `kill` command.

## Steps to Kill the Malicious Program

### 1. Run the Malicious Program

Inside the `worldbanc/private/bin/` directory, there is a program called `malicious.sh`. Sounds scary!

Execute the following command to run the malicious script in force mode:

```bash
./malicious.sh force
```

Try to stop it by pressing `CTRL+C`. You should see an output message indicating that the process cannot be stopped. **Copy** this output message, but do not submit it yet.

---

### 2. Find the Process ID (PID)

Open a new terminal window and run the following command to locate the PID of the running process:

```bash
ps aux | grep malicious.sh
```

This will return a list of processes that match "malicious.sh". You might see multiple lines:

```
user     12345  0.0  0.1  123456  7890 ?  S    12:34   0:00 ./malicious.sh force
user     12346  0.0  0.1  123456  7890 ?  S    12:34   0:00 grep --color=auto malicious.sh
```

Identify the correct PID from the first line (e.g., `12345`). Ignore the PID from the `grep` command itself.

---

### 3. Kill the Malicious Process

Once you have identified the correct PID, terminate the process using:

```bash
kill 12345
```

Replace `12345` with the actual PID you found.

If the process does not terminate, force it with:

```bash
kill -9 12345
```

---

### 4. Verify Termination

After running the `kill` command, check if your original terminal session is restored to a new prompt, confirming that the process has been successfully terminated.

## Additional Tips

- To view the column headers for better understanding, run:

  ```bash
  ps aux | head -n 1
  ```

- Be cautious when running `kill` commands to avoid terminating essential system processes.
