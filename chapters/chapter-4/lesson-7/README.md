# PATH Configuration for worldbanc.sh CLI Tool

This guide helps you set up the `worldbanc.sh` CLI tool so that it can be used from anywhere in your terminal session. By modifying your `PATH` environment variable, you'll ensure that the tool is always available after restarting your shell.

## Steps

### 1. Edit Your Shell Configuration File

Depending on the shell you are using, you will need to modify either `.zshrc` (for Zsh) or `.bashrc` (for Bash). Open the appropriate file for your shell in a text editor.

For **Zsh**, run:

```bash
nano ~/.zshrc
```

For **Bash**, run:

```bash
nano ~/.bashrc
```

### 2. Add the Export Command to the File

Scroll to the end of the file and add the following line to include the `worldbanc/private/bin` directory in your `PATH`:

```bash
export PATH=$PATH:/path/to/worldbanc/private/bin
```

Make sure to replace `/path/to/` with the actual path where the `worldbanc.sh` tool is located.

### 3. Restart Your Shell Session

After saving the changes to your shell configuration file, restart your terminal session for the changes to take effect.

You can restart your terminal by closing and reopening it or by running:

```bash
source ~/.zshrc  # For Zsh
# OR
source ~/.bashrc  # For Bash
```

### 4. Test the Configuration

To ensure the `worldbanc.sh` tool works globally, try running the tool from your home directory:

```bash
worldbanc.sh
```

If everything is set up correctly, the tool should run without any issues.

## Troubleshooting

- Ensure you are editing the correct shell configuration file (`.zshrc` for Zsh or `.bashrc` for Bash).
- Double-check the directory path to make sure it's correct.
- If the tool doesn't run, try running `echo $PATH` to confirm that the new directory was successfully added to your `PATH`.
