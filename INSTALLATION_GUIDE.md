# BCU Test Generator Professional v1.6.0 — Installation Guide

**Version:** 1.6.0 | **Released:** June 23, 2026 | **Status:** ✅ Production Ready

---

## Prerequisites

| Requirement | Details |
|-------------|---------|
| **Visual Studio Code** | 1.74.0 or higher |
| **BCU Framework** | Installed and accessible via `bcu` command in PATH |
| **Workspace** | Folder containing `.bcuproj` files |

> **Node.js is NOT required** — the extension is pre-compiled and ready to install.

---

## Installation

### Option 1: Install from VSIX via VS Code UI (Recommended)

1. Download [`bcu-test-generator-pro-1.6.0.vsix`](./bcu-test-generator-pro-1.6.0.vsix)
2. Open **VS Code**
3. Open **Extensions** panel (`Ctrl+Shift+X`)
4. Click the **`...`** menu → **Install from VSIX...**
5. Browse to the downloaded `.vsix` file and click **Install**
6. **Reload VS Code** when prompted

### Option 2: Install via Command Palette

1. Open **Command Palette** (`Ctrl+Shift+P`)
2. Type: **Extensions: Install from VSIX...**
3. Select the downloaded `.vsix` file

### Option 3: Install via Command Line

```bash
code --install-extension bcu-test-generator-pro-1.6.0.vsix
```

---

## Verify Installation

1. Open **Extensions** (`Ctrl+Shift+X`) — look for **BCU Test Generator Professional** showing as *Installed*, version **1.6.0**
2. Check the **Activity Bar** (left sidebar) for the 🚀 BCU icon
3. Open a workspace containing `.bcuproj` files — the tree view should populate automatically

---

## First Use

1. **Open workspace** containing `.bcuproj` files (`File → Open Folder`)
2. **Click the 🚀 BCU icon** in the Activity Bar
3. The extension auto-discovers your BCU project and source files
4. **Open the Dashboard** via Command Palette: `BCU Pro: Open Dashboard`
5. Select a function → click **Generate AI Test Cases** to start

---

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Extension not visible after install | Reload VS Code (`Ctrl+R`) |
| BCU icon missing in Activity Bar | Open a workspace with `.bcuproj` files |
| BCU commands not found in palette | Verify BCU Framework is installed and in PATH |
| Functions not detected | Check source files use `.c`/`.h` extensions and are in the workspace |
| Dashboard fails to load | Ensure VS Code version is 1.74.0+ |

**Enable debug logging** for detailed output:
```json
{
    "bcuTestGenerator.debugMode": true
}
```
Check output in **View → Output → BCU Test Generator**.

---

## Uninstall

**Via UI:** Extensions (`Ctrl+Shift+X`) → find *BCU Test Generator Professional* → **Uninstall**

**Via command line:**
```bash
code --uninstall-extension bcu-tools.bcu-test-generator-pro
```

---

## Extension Information

| Field | Value |
|-------|-------|
| **Name** | BCU Test Generator Professional |
| **Version** | 1.6.0 |
| **Publisher** | bcu-tools |
| **Author** | Andrew Nelson (MS/ESS12-PS) |
| **Organization** | Bosch Global Software Technologies |
| **License** | BGSW |
| **VS Code** | 1.74.0+ |

---

*For usage instructions see [README.md](./README.md) · For release details see [RELEASE_NOTES.md](./RELEASE_NOTES.md)*
