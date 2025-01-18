## Common Unix Shells

### 1. **sh** - The Bourne Shell

- The original Unix shell.
- POSIX-compliant and very basic.
- Lacks advanced features and conveniences.

### 2. **bash** - The Bourne Again Shell

- Most popular shell on Linux systems.
- Builds on `sh` with many extra features.
- Default on many Linux distributions.

### 3. **zsh** - The Z Shell

- Default shell on macOS.
- Combines features from `bash` with advanced customization.
- Offers features like better autocompletion and plugins.

### Compatibility

Both **bash** and **zsh** are **sh-compatible**, meaning:

- They can run `.sh` scripts.
- They offer additional features beyond the basic `sh` shell.

### Shell Usage by Platform

- **Ubuntu on WSL:** Likely using **bash**.
- **macOS:** Default is **zsh**.
- **Raw Linux Installations:** Typically **bash**, but can vary.

For most use cases, the differences between **bash** and **zsh** are minimal, and scripts written for one will usually run on the other.
