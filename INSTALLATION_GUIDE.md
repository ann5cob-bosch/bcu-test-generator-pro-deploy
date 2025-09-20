# BCU Test Generator Professional v1.2.0 - Installation Guide

## Overview
BCU Test Generator Professional is a Visual Studio Code extension designed for BCU (Build Configuration Utility) project management and AI-powered test case generation. This guide provides step-by-step installation instructions and prerequisites.

## Prerequisites

### 1. System Requirements
- **Operating System**: Windows 10/11 (primary support), Linux, macOS
- **Memory**: Minimum 4GB RAM, Recommended 8GB+
- **Storage**: At least 500MB free space
- **Network**: Internet connection for extension marketplace access

### 2. Required Software

#### Visual Studio Code
- **Version**: 1.74.0 or higher
- **Download**: [https://code.visualstudio.com/](https://code.visualstudio.com/)
- **Installation**: Follow the standard VS Code installation process

#### Node.js (Optional - for development)
- **Version**: 16.x or higher
- **Download**: [https://nodejs.org/](https://nodejs.org/)
- **Purpose**: Required only if you plan to modify or contribute to the extension

#### BCU Framework
- **Requirement**: BCU (Build Configuration Utility) must be installed and accessible
- **Verify Installation**: Ensure `bcu.cmd` or `bcu` command is available in your system PATH
- **Project Files**: You should have access to `.bcuproj` files

#### Python (Optional - for advanced features)
- **Version**: 3.8 or higher
- **Purpose**: Required for AI-powered test case generation features
- **Packages**: `requirements.txt` included in extension for automatic setup

### 3. Workspace Requirements
- **BCU Project**: At least one valid `.bcuproj` file in your workspace
- **Source Files**: C/C++ source files linked to your BCU project
- **Test Cases**: Existing test case files (optional, can be generated)

## Installation Methods

### Method 1: Install from VSIX Package (Recommended)

1. **Download the Package**
   ```
   Package: bcu-test-generator-pro.vsix
   Size: 337.42KB
   ```

2. **Open Visual Studio Code**
   - Launch VS Code
   - Ensure you have the latest version (1.74.0+)

3. **Install from VSIX**
   - Open Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
   - Type: `Extensions: Install from VSIX...`
   - Select the command and click
   - Browse to `bcu-test-generator-pro.vsix`
   - Click "Install"

4. **Alternative Installation Method**
   - Go to Extensions view (`Ctrl+Shift+X`)
   - Click the "..." menu (More Actions)
   - Select "Install from VSIX..."
   - Choose the `bcu-test-generator-pro.vsix` file

5. **Reload VS Code**
   - When prompted, click "Reload" or restart VS Code
   - The extension will be activated automatically

### Method 2: Manual Installation (Advanced Users)

1. **Extract Package Contents**
   ```bash
   # Create extension directory
   mkdir ~/.vscode/extensions/bcu-tools.bcu-test-generator-pro-1.2.0
   
   # Extract VSIX contents
   unzip bcu-test-generator-pro.vsix -d ~/.vscode/extensions/bcu-tools.bcu-test-generator-pro-1.2.0
   ```

2. **Restart VS Code**
   - Close all VS Code instances
   - Reopen VS Code to load the extension

## Post-Installation Setup

### 1. Verify Installation
- Open Command Palette (`Ctrl+Shift+P`)
- Type: `BCU Pro` - you should see BCU Test Generator commands
- Check Activity Bar for the rocket icon (🚀)

### 2. Configure BCU Path (if needed)
- Open VS Code Settings (`Ctrl+,`)
- Search for "BCU"
- Set the correct path to your BCU installation

### 3. Open a BCU Project
- Open a workspace containing `.bcuproj` files
- The extension will automatically detect BCU projects
- Click the BCU Test Generator icon in the Activity Bar

### 4. Access the Dashboard
- Use Command Palette: `BCU Pro: Open BCU Test Generator Dashboard`
- Or click the rocket icon in the Activity Bar
- The webview dashboard should open with project information

## Feature Activation

### Core Features (Available Immediately)
- ✅ BCU Project Detection
- ✅ Source File Analysis
- ✅ Function Detection
- ✅ Webview Dashboard
- ✅ Execution Controls with Toggle Options

### Advanced Features (Require Setup)
- **AI Test Generation**: Requires Python installation
- **Coverage Analysis**: Requires BCU framework with coverage support
- **Real-time Execution**: Requires valid BCU project configuration

## Troubleshooting

### Common Installation Issues

#### Extension Not Loading
```
Problem: Extension doesn't appear after installation
Solution: 
1. Restart VS Code completely
2. Check Extensions view to confirm installation
3. Look for error messages in Developer Console (Help > Toggle Developer Tools)
```

#### BCU Commands Not Found
```
Problem: BCU-related commands don't appear
Solution:
1. Ensure you have a .bcuproj file in your workspace
2. Verify BCU framework is installed
3. Check VS Code Output panel for BCU Test Generator logs
```

#### Dashboard Not Opening
```
Problem: Webview dashboard fails to load
Solution:
1. Check VS Code version (must be 1.74.0+)
2. Try reloading the window (Ctrl+R)
3. Check browser settings if using VS Code in browser
```

#### Function Detection Issues
```
Problem: C functions not detected properly
Solution:
1. Ensure source files are in the correct directory structure
2. Check file extensions (.c, .h)
3. Use the "Detect and Add Source Files" command
```

### Performance Issues

#### Slow Function Scanning
```
Solution:
1. Use incremental scanning (enabled by default)
2. Exclude large directories from workspace
3. Increase VS Code memory allocation if needed
```

#### Large Project Handling
```
Solution:
1. Enable background scanning
2. Use manual refresh instead of auto-refresh
3. Close unnecessary files/tabs
```

## Verification Checklist

After installation, verify these features work:

- [ ] Extension appears in Extensions list
- [ ] BCU Test Generator icon visible in Activity Bar
- [ ] Command Palette shows "BCU Pro" commands
- [ ] Dashboard opens without errors
- [ ] BCU projects are detected automatically
- [ ] Source files can be browsed
- [ ] Functions are detected and listed
- [ ] Toggle buttons work in execution tab
- [ ] Test execution can be initiated (with valid BCU setup)

## Support and Documentation

### Getting Help
- **Issues**: Report problems at [GitHub Issues](https://github.com/bcu-tools/bcu-test-generator-pro/issues)
- **Documentation**: See README.md for detailed usage instructions
- **Updates**: Check VS Code Extensions for updates

### Additional Resources
- **BCU Framework Documentation**: Refer to your BCU installation guide
- **Python Setup**: See `python-tools/requirements.txt` for Python dependencies
- **Templates**: Located in `templates/` directory for test case generation

### Extension Information
- **Name**: BCU Test Generator Professional
- **Version**: 1.2.0
- **Publisher**: bcu-tools
- **License**: Bosch Global Software Technologies
- **Author**: Andrew Nelson (MS/ESS12-PS)

---

## Quick Start

Once installed:

1. **Open Workspace** with `.bcuproj` files
2. **Click BCU Icon** (🚀) in Activity Bar
3. **Open Dashboard** for project overview
4. **Configure Toggles** for execution preferences
5. **Execute Tests** with real-time monitoring

**Status**: ✅ Ready for Production Use

For detailed usage instructions, see the main README.md file.
