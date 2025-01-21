# Package Managers

A package manager is a software tool that helps you install other software. Its primary functions include:

- Downloading software from official sources
- Installing software
- Updating software
- Removing software
- Managing dependencies

As a developer, you'll frequently use package managers to get access to the software you need to get your work done.

## APT (Ubuntu)

APT, or "Advanced Package Tool", is the primary package manager for Ubuntu. Although other package managers can be used on Ubuntu, APT is the default and most common.

If you're using WSL and Ubuntu, you'll be using APT. To check if APT is installed, run the following command:

```sh
apt --version
```

## Brew (macOS)

There isn't a "default" package manager for macOS. The most popular (but unofficial) package manager is Homebrew.

If you're on macOS and don't have Homebrew installed, you can install it by running the following command:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

For more information, visit the [Homebrew website](https://brew.sh).

## Assignment: Installing Neovim

Neovim is a hyperextensible and newer version of Vim, which itself is a modernized version of Vi, a popular command line text editor.

### WSL/Ubuntu Instructions

1. Update APT to ensure it installs the latest version of Neovim:

   ```sh
   sudo apt update
   ```

2. Install Neovim:

   ```sh
   sudo apt install neovim
   ```

### macOS Instructions

If you're using Homebrew on Mac, you can install Neovim by running:

```sh
brew install neovim
```

### Other Installation Methods

If the above methods don't work, consider exploring other installation methods available on the official [Neovim website](https://neovim.io).

## Check Installation

Once Neovim is installed, verify the installation by running:

```sh
nvim --version
```
