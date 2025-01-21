# Installing and Using LSD with Webi

## Introduction

[Webi](https://webinstall.dev/) is an easy way to install command-line tools directly from the web without the need for traditional package managers like `apt` or `brew`. In this guide, we will install `lsd` (LSDeluxe), a modern replacement for the `ls` command, and explore its features.

## Installation

### Step 1: Install LSD

To install `lsd` using Webi, follow these steps:

1. Visit [LSDeluxe on Webi](https://webinstall.dev/lsd).
2. Copy the installation command based on your operating system.

#### For Linux/WSL/macOS:

```sh
curl -sS https://webi.sh/lsd | sh
```

The command downloads and installs `lsd` without requiring additional package managers.

### Step 2: Verify Installation

Once installed, verify by running:

```sh
lsd --version
```

## Usage

### Step 1: List Files in a Directory

Navigate to the `worldbanc/private/transactions` directory and run:

```sh
lsd
```

This command lists all files in the specified directory with enhanced visuals.

### Step 2: Display Files in Tree Format

To display files in a tree-like structure within the `worldbanc/private` directory, run:

```sh
lsd --tree
```

### Step 3: Classic Tree View

For a more traditional look, combine the `--tree` and `--classic` flags within the `worldbanc/private/transactions` directory:

```sh
lsd --tree --classic
```

## Optional: Enable Icons

To enhance the display with icons, install a Nerd Font and update your terminal font settings:

1. Download a Nerd Font from [NerdFonts.com](https://www.nerdfonts.com/).
2. Install the font and apply it in your terminal settings.
3. Run `lsd` again to see icons in file listings.

## Conclusion

You have successfully installed and tested `lsd` using Webi. Enjoy a modern and feature-rich alternative to the classic `ls` command!
