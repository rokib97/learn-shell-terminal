# Users and Superuser Privileges

## Users in Unix-like Systems

Unix-like systems support multiple users, each with their own home directory, files, and permissions.

- On most personal computers today, there's typically only one user.
- Historically, multiple users often shared a single machine or accessed it remotely over a network.

## `sudo`: Superuser Access

The `sudo` command allows you to run programs with superuser (administrator) privileges.

- **sudo** stands for **"superuser do"**.
- It requires a password with superuser rights, which you likely have if you're the only user on your machine.

> ⚠ **Warning:** `sudo` gives full control over the system. Misuse can lead to system damage. Commands in this course are safe, but always review unfamiliar commands before using `sudo`.

**Fun Fact:**  
Some pronounce `sudo` as **"sue-doo"**, but it's commonly pronounced as **"sue-dough"**.

---

## Assignment: Verify Superuser Access

### 1. Check Your Current User

Run the following command to display your current username:

```bash
whoami
```

### 2. Check Superuser Access

Run the same command with `sudo` to check if you can execute commands as the root user:

```bash
sudo whoami
```

- You’ll be prompted to enter your password.
- If successful, the output should display:

```
root
```

### 3. **Verification**

After running the command, if `"root"` is displayed, your superuser access is verified, and the task is complete.

If not, ensure you entered your password correctly and try again.
