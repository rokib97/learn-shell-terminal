# Environment Variables and Script Execution Guide

## Overview

This document explains how to set and use environment variables in the shell, particularly for executing scripts that rely on them. It also details how to complete the assignment involving the `warn.sh` script in the `worldbanc/private/bin` directory.

## Understanding Environment Variables

- **Local Variable:** Only available in the current shell session.  
  Example:

  ```bash
  name="Lane"
  echo $name  # Output: Lane
  ```

- **Environment Variable:** Accessible to all programs and scripts run in the shell.  
  Example:
  ```bash
  export NAME="Lane"
  echo $NAME  # Output: Lane
  ```

## Viewing Environment Variables

List all currently set environment variables:

```bash
env
```

## Setting Environment Variables

1. **Persistent for the session:**

   ```bash
   export WARN_MESSAGE="The auditor is here"
   export WARN_FROM_NAME="Your worst nightmare"
   ```

2. **Temporary for a single command:**
   ```bash
   WARN_MESSAGE="The auditor is here" WARN_FROM_NAME="Your worst nightmare" ./warn.sh
   ```

## Running the Script

1. **Navigate to the script directory:**

   ```bash
   cd worldbanc/private/bin
   ```

2. **Make the script executable (if needed):**

   ```bash
   chmod +x warn.sh
   ```

3. **Run the script:**

   ```bash
   ./warn.sh
   ```

4. **Expected Output:**
   The script should print a formatted warning message that includes the values of `WARN_MESSAGE` and `WARN_FROM_NAME`. Example output:
   ```
   ************************************
   WARNING: The auditor is here
   - From: Your worst nightmare
   ************************************
   ```

## Conclusion

By correctly setting the required environment variables and running the script, you should see the warning message formatted with the worldbanc branding. Use either the `export` method for session persistence or inline variable declaration for temporary use.
