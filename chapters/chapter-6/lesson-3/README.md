# Package Manager Review

Apt and Brew aren't the only package managers out there. There are many, many more, though they do happen to be two of the most popular, especially on Linux and macOS.

## How Does a Package Manager Work?

When you type a command like:

```
apt install neovim
```

the package manager will:

1. **Check if the package is already installed.**
2. **Download the package** from a repository if it's not installed.
3. **Install the package** on your computer.
4. **Install dependencies** that the package needs to run.
5. **Update the PATH**, if necessary, to make the package accessible from the command line.

A good package manager keeps track of:

- Installed packages.
- Their versions.
- Ensuring a tidy filesystem without redundant installations.

This helps avoid installing multiple versions of the same package and keeps your system organized.

### Checking Package Installation

To check where a package is installed on your system, you can use the `which` command. For example:

```
which nvim
```

This will return the path to the installed `nvim` executable, showing where it resides in your filesystem.
