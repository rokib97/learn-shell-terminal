# WorldBanc Setup Guide

## Understanding Filepaths

A **filepath** is a string that describes the location of a file or directory on your computer. An example of a filepath looks like this:

```
/Users/wagslane
```

### Breakdown of the Filepath:

- **/** : Represents the **root directory**, the topmost level of the filesystem.
- **Users** : A directory inside the root directory.
- **wagslane** : A directory inside the Users directory.

This structure represents a path two levels down from the root directory:

```
root
└── Users
    └── wagslane
```

---

## Assignment: Download and Set Up the WorldBanc Directory

### Step 1: Download the WorldBanc Repository

Run the following commands in your terminal to download and set up the **worldbanc** directory:

```bash
# Download the worldbanc directory from GitHub
curl -L https://github.com/bootdotdev/worldbanc/archive/refs/heads/main.zip -o worldbanc.zip

# Unzip the downloaded file
unzip worldbanc.zip

# Remove the zip file to clean up
rm worldbanc.zip

# Rename the extracted folder to 'worldbanc'
mv worldbanc-main worldbanc

# Change ownership to the current user
sudo chown -R $(whoami) worldbanc

# Set proper permissions
sudo chmod -R 755 worldbanc
```

### Step 2: Verify the Setup

1. **List Directory Contents**  
   Run the following command to verify the **worldbanc** directory exists:

   ```bash
   ls
   ```

   You should see `worldbanc` in the output.

2. **Navigate into the worldbanc Directory**  
   Change into the directory:

   ```bash
   cd worldbanc
   ```

3. **List Contents of worldbanc**  
   Verify its contents:

   ```bash
   ls
   ```

---

## Troubleshooting

- **curl or unzip not installed?**  
  Install them using:

  ```bash
  sudo apt install unzip
  sudo apt install curl
  ```

- **Can't paste in the terminal?**  
  Use **Ctrl + Shift + V** to paste commands.

If any issues occur, revisit the steps to redownload and set up the directory.
