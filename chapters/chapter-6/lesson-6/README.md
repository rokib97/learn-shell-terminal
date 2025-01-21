# Setting Up WSL in VS Code

If you're on Mac or Linux (non-WSL), you can skip this step. However, if you're using Windows with WSL, follow these steps to set up VS Code to work seamlessly with your Linux environment. This setup will allow you to leverage the full power of the Linux filesystem within VS Code.

## Steps to Set Up WSL in VS Code

### 1. Install the WSL Extension

1. Open **VS Code**.
2. Navigate to the **"Extensions"** menu on the left-hand toolbar.
3. Search for **"WSL"** and install the extension created by Microsoft.

### 2. Connect VS Code to WSL

1. Look at the **bottom-left corner** of VS Code for a green or blue button.
2. Click on it and select **"Connect to WSL using Distro"**.
3. Choose **"Ubuntu"** or your preferred WSL distribution.
4. A new VS Code window will open, connected to your WSL environment.

> **Tip:** Pin this new WSL-enabled VS Code window to your taskbar for easy access in the future.

### 3. Open Your Project Directory

1. In the WSL-enabled VS Code window, go to **"File" -> "Open Folder"**.
2. Navigate to your **worldbanc** directory and open it.
3. Your project files and directories should now be visible in the sidebar.

## Important Notes

- Always use the WSL-enabled VS Code window to access your Linux filesystem.
- Avoid using the "regular" VS Code window, as it won't have access to your WSL environment.
- For more details, refer to the [VS Code WSL extension Getting Started page](https://code.visualstudio.com/docs/remote/wsl).

---

**Congratulations on completing the course!**
