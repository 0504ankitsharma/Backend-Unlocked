### For Windows Users:
1. **Download the Installer:**
   - Visit the [Node.js official website](https://nodejs.org/).
   - Choose the Windows Installer (`.msi` file) for either the LTS (Long-Term Support) version or the current version.

2. **Run the Installer:**
   - Open the downloaded `.msi` file and follow the installation steps.
   - Ensure the option to install npm is checked.
   - Accept the license agreement and select the default settings.

3. **Verify the Installation:**
   - Open **Command Prompt** or **PowerShell**.
   - Run the following commands to check the installed versions:
     ```bash
     node -v
     npm -v
     ```
   - You should see version numbers for both Node.js and npm.

### For macOS Users:
1. **Using Homebrew (Recommended Method):**
   - Open **Terminal**.
   - First, check if Homebrew is installed by running:
     ```bash
     brew --version
     ```
     If not installed, install Homebrew using:
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```

   - Once Homebrew is installed, install Node.js and npm by running:
     ```bash
     brew install node
     ```

2. **Verify the Installation:**
   - Run the following in **Terminal** to confirm installation:
     ```bash
     node -v
     npm -v
     ```

### Alternative for macOS (Manual Installation):
1. **Download the Installer:**
   - Go to the [Node.js official website](https://nodejs.org/).
   - Download the `.pkg` file for macOS.

2. **Run the Installer:**
   - Double-click the downloaded `.pkg` file and follow the prompts to install.

3. **Verify the Installation:**
   - Open **Terminal** and type:
     ```bash
     node -v
     npm -v
     ```

### Important Tips:
- **LTS vs Current Version**: LTS versions are more stable, so they are recommended for most users unless you need the latest features.
- **Node.js Comes with npm**: Installing Node.js also installs npm by default.
- **Troubleshooting**: If you face permission issues when installing npm packages globally, consider using a version manager like `nvm` to manage Node.js versions and avoid using `sudo`.