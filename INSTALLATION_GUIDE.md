# BCU Test Generator Professional v1.6.0 - Installation Guide

**Last Updated:** June 23, 2026  
**Version:** 1.6.0  
**Status:** ✅ Production Ready

---

## 📋 Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation Methods](#installation-methods)
3. [Verification](#verification)
4. [First Steps](#first-steps)
5. [Troubleshooting](#troubleshooting)
6. [Uninstallation](#uninstallation)

---

## Prerequisites

### For End Users

- **Visual Studio Code**: Version 1.74.0 or higher
- **BCU Framework**: Installed and configured in your environment
- **Workspace**: Containing `.bcuproj` files to manage
- **Storage**: ~50MB for extension and dependencies

**Note:** Node.js is NOT required - the extension is pre-compiled and ready to use.

### For Developers

- **Visual Studio Code**: Version 1.74.0 or higher
- **Node.js**: Version 16.x or higher
- **npm**: Version 7.x or higher (comes with Node.js)
- **Git**: For version control (optional)
- **TypeScript**: Understanding of TypeScript helpful for contributions

### System Requirements

- **OS**: Windows, macOS, or Linux
- **RAM**: Minimum 2GB (4GB recommended for large projects)
- **Disk Space**: ~100MB for full development setup

---

## Installation Methods

### Method 1: Install from VS Code Extensions Marketplace (Recommended)

1. Open **VS Code**
2. Navigate to **Extensions** (Ctrl+Shift+X / Cmd+Shift+X)
3. Search for **"BCU Test Generator Professional"**
4. Click **Install** button
5. Wait for installation to complete
6. **Reload VS Code** when prompted (or manually with Ctrl+R)

### Method 2: Manual Installation from VSIX File

#### Step 1: Download the Extension

Download the latest `.vsix` file:
- **Latest Release**: `bcu-test-generator-pro-1.6.0.vsix`
- **Location**: [Releases Page](https://github.boschdevcloud.com/ANN5COB/bcu-test-generator-pro/releases)

#### Step 2: Install via VS Code UI

1. Open **VS Code**
2. Open **Extensions** (Ctrl+Shift+X / Cmd+Shift+X)
3. Click the **"..."** menu (top-right of Extensions panel)
4. Select **"Install from VSIX..."**
5. Navigate to and select the downloaded `.vsix` file
6. Click **Install**
7. **Reload VS Code** when prompted

#### Step 3: Verify Installation

Check that the extension appears in your Extensions list and shows as "Installed".

### Method 3: Command Line Installation

#### Windows PowerShell

```powershell
# Navigate to the extension directory
cd "C:\path\to\BCUTestGenTool_VSCodeExtn"

# Install the extension
code --install-extension "./bcu-test-generator-pro-1.6.0.vsix"
```

#### macOS / Linux Terminal

```bash
# Navigate to the extension directory
cd /path/to/BCUTestGenTool_VSCodeExtn

# Install the extension
code --install-extension "./bcu-test-generator-pro-1.6.0.vsix"
```

### Method 4: Build from Source

#### Prerequisites
- Node.js 16.x or higher
- npm 7.x or higher
- Git

#### Steps

```bash
# 1. Clone the repository
git clone https://github.boschdevcloud.com/ANN5COB/bcu-test-generator-pro.git
cd BCUTestGenTool_VSCodeExtn

# 2. Install dependencies
npm install

# 3. Compile TypeScript
npm run compile

# 4. Package the extension
npm run package
# or install vsce first: npm install -g @vscode/vsce
# then: vsce package

# 5. Install the generated VSIX
code --install-extension bcu-test-generator-pro-1.6.0.vsix
```

---

## Verification

### Verify Installation Success

1. **Check Extensions List**
   - Open Extensions (Ctrl+Shift+X)
   - Search for "BCU Test Generator Professional"
   - Should show as **Installed** (not "Install" button)
   - Version should be **1.6.0**

2. **Check Activity Bar**
   - Look for the **BCU icon** (🚀) in the VS Code Activity Bar (left sidebar)
   - Click to open the BCU Test Generator panel

3. **Verify Activation**
   - Open a workspace containing `.bcuproj` files
   - Wait 2-3 seconds for extension to activate
   - You should see the BCU tree view populate with projects

### Verify BCU Framework Setup

1. Open terminal in VS Code (Ctrl+`)
2. Test BCU command availability:

```bash
# Windows
bcu --version

# macOS / Linux
bcu --version
```

3. Should return BCU version information (e.g., "BCU 2.5.1")

---

## First Steps

### Initial Setup Workflow

1. **Open BCU Project Workspace**
   ```
   File → Open Folder → Select folder containing .bcuproj files
   ```

2. **Activate Extension**
   ```
   Wait 2-3 seconds for extension to activate
   OR click BCU icon (🚀) in Activity Bar
   ```

3. **Browse Projects**
   ```
   In BCU Test Generator panel → Right-click → "Refresh"
   OR use "Browse BCU Project" command
   ```

4. **Select Project**
   ```
   Click on project in tree view
   Extension automatically detects source files
   ```

5. **Start Test Generation**
   ```
   Select a function → "Generate AI Test Cases"
   Review generated templates
   Execute tests with the dashboard
   ```

### Configuration (Optional)

Create or edit workspace settings in `.vscode/settings.json`:

```json
{
  "bcuTestGenerator.backgroundValidation": true,
  "bcuTestGenerator.debugMode": false,
  "bcuTestGenerator.maxFileSize": 1048576,
  "bcuTestGenerator.templatePath": "./templates"
}
```

**Configuration Options:**

| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| `backgroundValidation` | boolean | true | Enable background BCU project validation |
| `debugMode` | boolean | false | Enable debug logging in output |
| `maxFileSize` | number | 1048576 | Maximum file size for parsing (bytes) |
| `templatePath` | string | "./templates" | Path to custom templates (relative to workspace) |

---

## Troubleshooting

### Extension Won't Install

**Problem:** Installation fails with error message

**Solutions:**
1. Ensure VS Code is closed
2. Download the VSIX file again (may be corrupted)
3. Try installing from command line:
   ```bash
   code --install-extension bcu-test-generator-pro-1.6.0.vsix
   ```
4. Check VS Code version (must be 1.74.0 or higher)

### Extension Won't Activate

**Problem:** BCU icon doesn't appear in Activity Bar, no tree view shows

**Solutions:**
1. Ensure workspace contains `.bcuproj` files
2. Reload VS Code (Ctrl+R / Cmd+R)
3. Check VS Code output for errors:
   - View → Output → Select "BCU Test Generator" from dropdown
4. Restart VS Code completely
5. Uninstall and reinstall extension

### BCU Command Not Found

**Problem:** Extension says "BCU not found" or "bcu command not recognized"

**Solutions:**
1. Verify BCU is installed:
   ```bash
   bcu --version
   ```
2. Check BCU is in system PATH:
   - Windows: System Properties → Environment Variables → PATH
   - macOS/Linux: Check `$PATH` contains BCU bin directory
3. Restart VS Code after fixing PATH
4. Verify BCU version (must be compatible - typically 2.5.0 or higher)

### Projects Not Detected

**Problem:** No projects appear in tree view even with .bcuproj files present

**Solutions:**
1. Refresh the view:
   - Right-click in BCU tree → "Refresh"
   - Or press F5 with tree view focused
2. Verify .bcuproj files exist in workspace
3. Check file permissions (must be readable)
4. Try closing and reopening the workspace
5. Check output for parsing errors (View → Output)

### Performance Issues

**Problem:** Extension slow, UI laggy, or high memory usage

**Solutions:**
1. Disable background validation (temporarily):
   ```json
   "bcuTestGenerator.backgroundValidation": false
   ```
2. Increase file size limit to skip large files:
   ```json
   "bcuTestGenerator.maxFileSize": 2097152
   ```
3. Close other VS Code extensions
4. Check available disk space
5. Restart VS Code

### Network Connectivity Issues

**Problem:** Extension shows network error or can't connect

**Solutions:**
1. This is non-critical for core functionality
2. Extension operates offline (network is optional)
3. Check internet connection
4. Try toggling internet and restarting extension
5. Network errors are logged but don't prevent operation

---

## Uninstallation

### Remove via VS Code UI

1. Open **Extensions** (Ctrl+Shift+X / Cmd+Shift+X)
2. Search for **"BCU Test Generator Professional"**
3. Click **Uninstall** button
4. **Reload VS Code** when prompted

### Remove via Command Line

```bash
code --uninstall-extension bcu-tools.bcu-test-generator-pro
```

### Manual Removal (Advanced)

**Windows:**
```powershell
Remove-Item "$env:USERPROFILE\.vscode\extensions\bcu-tools.bcu-test-generator-pro-*" -Recurse
```

**macOS/Linux:**
```bash
rm -rf ~/.vscode/extensions/bcu-tools.bcu-test-generator-pro-*
```

---

## Getting Help

### Documentation
- **Main Documentation**: See [README.md](./README.md)
- **Changelog**: See [CHANGELOG.md](./CHANGELOG.md)
- **Release Notes**: See [RELEASE_NOTES_v1.6.0.md](./RELEASE_NOTES_v1.6.0.md)

### Support Channels
- **Issues**: [GitHub Issues](https://github.boschdevcloud.com/ANN5COB/bcu-test-generator-pro/issues)
- **Email**: [Support](mailto:andrew.nelson@bosch.com)
- **Documentation**: [BCU Documentation](https://bosch-internal-docs.com/bcu/)

### Reporting Bugs

When reporting issues, please include:
1. VS Code version (`Help → About`)
2. Extension version (`Extensions → BCU Test Generator Pro → Details`)
3. BCU version (`bcu --version`)
4. Error message (copy from Output panel)
5. Steps to reproduce

---

## Version History

| Version | Release Date | Status |
|---------|--------------|--------|
| 1.6.0 | June 23, 2026 | ✅ Current (Production) |
| 1.5.0 | November 5, 2025 | Archived |
| 1.0.0 | 2024 | Legacy |

---

**Ready to get started?** 🚀

1. [Install the extension](#installation-methods)
2. [Verify installation](#verification)
3. [Follow first steps](#first-steps)
4. [Check README.md](./README.md) for usage documentation

---

*For the latest updates, visit [GitHub Repository](https://github.boschdevcloud.com/ANN5COB/bcu-test-generator-pro)*
