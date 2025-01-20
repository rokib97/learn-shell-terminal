# Exit Codes in Shell Scripts

Exit codes (also known as return codes or status codes) are used by programs to indicate whether they executed successfully or encountered an error.

## Exit Code Meanings

- **0**: Indicates successful execution.
- **Non-zero (1-255)**: Indicates an error occurred.
  - **1**: Common "catch-all" error code, used when no specific error code is defined.

Programs that execute other programs often check exit codes to determine the next steps, such as logging errors or restarting services.

## Checking Exit Codes

In the shell, the exit code of the last executed command can be accessed using the special variable `$?`.

### Example Usage

```sh
ls ~
echo $?  # Expected output: 0 (success)

ls /does/not/exist
echo $?  # Expected output: 1 (error)
```

## Assignment Instructions

1. Run the script `private/bin/warn.sh` without setting the required environment variables (`WARN_MESSAGE` and `WARN_FROM_NAME`).
2. Check the exit code using the `echo $?` command.

## Helpful Commands

To remove an environment variable:

```sh
unset ENV_VAR_NAME
```

Alternatively, set it to an empty string:

```sh
export ENV_VAR_NAME=""
```

## Additional Notes

- Always check exit codes when scripting automation or debugging.
- Some programs may use specific exit codes to indicate different error types.
- Use `man <command>` to check if specific exit codes are documented.
