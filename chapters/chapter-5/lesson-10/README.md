# Interrupting a Running Program

Sometimes, programs may get stuck, requiring manual intervention to stop them. Common reasons for needing to stop a running program include:

- A typo in the command leading to unexpected behavior.
- An attempt to access the internet when no connection is available.
- Processing too much data, leading to long wait times.
- A bug in the program causing it to hang indefinitely.

## How to Stop a Running Program

To stop a running program, you can press `Ctrl + C`. This keyboard shortcut sends a "SIGINT" (Signal Interrupt) to the running process, instructing it to terminate.

---

## Assignment Instructions

In the `worldbanc/private/bin/` directory, there is a script named `malicious.sh`. As a responsible security auditor, you are tasked with analyzing it.

### Steps to follow:

1. Navigate to the directory:

   ```bash
   cd worldbanc/private/bin/
   ```

2. Run the `malicious.sh` script:

   ```bash
   ./malicious.sh
   ```

3. Observe the program's behavior.

4. Use `Ctrl + C` to send a SIGINT signal and stop the program.

By following these steps, you can safely explore the script's functionality while maintaining control over the execution process.
