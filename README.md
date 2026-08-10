# BCU Test Generator Professional

<div align="center">

![BCU Test Generator Pro Logo](https://img.shields.io/badge/BCU-Test%20Generator%20Pro-blue?style=for-the-badge&logo=visual-studio-code)

**BCU project management and AI-powered test case generation for Visual Studio Code**

[![Version](https://img.shields.io/badge/version-1.7.0-blue.svg)](https://github.boschdevcloud.com/ANN5COB/bcu-test-generator-pro)
[![License](https://img.shields.io/badge/license-BGSW-green.svg)](LICENSE)
[![VS Code](https://img.shields.io/badge/VS%20Code-1.74.0%2B-brightgreen.svg)](https://code.visualstudio.com/)

[📋 Features](#-features) • [🚀 Installation](#-installation) • [▶️ Usage](#%EF%B8%8F-usage) • [⌨️ Commands](#%EF%B8%8F-commands) • [🔄 Changelog](#-changelog)

</div>

---

## 📋 Features

### 🧠 AI-Powered Test Generation
- Seamless GitHub Copilot integration with BCU-specific prompt templates
- 2-step workflow: **Analysis** → **Implementation**
- Production-ready test cases using BCU 2.5.1 patterns
- Cyclomatic complexity analysis for smarter test coverage planning

### 🎯 Smart C Function Analysis
- Automatic detection of C functions with AUTOSAR compliance support
- Support for function pointers and complex callback types
- Background file scanning with performance safety constraints

### 🎮 Professional Dashboard
- Card-based WebView dashboard with multi-tab layout
- Tabs: Project Overview · Execution · Results · Review
- Live execution progress tracking
- Adapts to VS Code dark/light themes

### ⚡ BCU Execution Controls
- Toggle switches for BCU command parameters:
  - 🔧 **Function Mocking** (`-calltrace`) — enable/disable call tracing
  - 📊 **Code Coverage** (`-ctc`) — toggle coverage analysis
  - 🚫 **No DSM Library** (`-nodsm`) — exclude DSM library
  - 📦 **Archive** — zip result packaging
- Three execution modes:
  - **Execute All** — run all test cases
  - **Execute Selected** — run chosen test cases
  - **Execute Function** — run tests for a single function

### 🔍 Project Management
- Automatic `.bcuproj` file discovery and validation
- C source file detection and function parsing
- Multi-scenario test report support (cfg2, cfg3, maxcfg, etc.)
- Real-time file watching for project changes

---

## 🚀 Installation

### Prerequisites
- **Visual Studio Code** 1.74.0 or higher
- **BCU Framework** installed and in your system PATH
- A workspace containing `.bcuproj` files

> Node.js is **not required** — the extension is pre-compiled.

### Install from VSIX

1. Download [`bcu-test-generator-pro-1.7.0.vsix`](./bcu-test-generator-pro-1.7.0.vsix)
2. Open VS Code → **Extensions** (`Ctrl+Shift+X`)
3. Click **`...`** → **Install from VSIX...**
4. Select the downloaded file and click **Install**
5. Reload VS Code when prompted

### Install via Command Line

```bash
code --install-extension bcu-test-generator-pro-1.7.0.vsix
```

---

## ▶️ Usage

### Getting Started

1. **Open your BCU project workspace** — folder containing `.bcuproj` files
2. **Click the BCU icon** (🚀) in the Activity Bar — the extension activates automatically
3. **Browse / select your BCU project** from the tree view
4. The extension auto-detects source files and parses C functions

### Generating Test Cases

1. Select a function from the dashboard
2. Click **Generate AI Test Cases**
3. Review the generated prompt in the editor (GitHub Copilot chat opens)
4. Accept and refine the generated test code
5. Run tests using the execution controls

### BCU Project Structure Expected

```
your-bcu-project/
├── your_project.bcuproj     ← required
├── src/                     ← C source files
│   ├── module.c
│   └── module.h
└── My/                      ← BCU test output
    ├── my_project_ut.c
    └── stub_functions.c
```

### Two-Step AI Workflow

| Step | Action | Description |
|------|--------|-------------|
| 1 | **Analysis** | Copilot analyzes the function signature, dependencies, and test scenarios |
| 2 | **Implementation** | Copilot generates production-ready BCU test code and stubs |

---

## ⌨️ Commands

Access via **Command Palette** (`Ctrl+Shift+P`) and type `BCU`:

| Command | Description |
|---------|-------------|
| `BCU Pro: Open Dashboard` | Launch the main WebView dashboard |
| `BCU Pro: Browse BCU Project` | Select and validate a BCU project |
| `BCU Pro: Generate AI Test Cases` | Generate tests for the selected function |
| `BCU Pro: Execute All Test Cases` | Run the full test suite |
| `BCU Pro: Detect Source Files` | Scan workspace for C source files |
| `BCU Pro: Refresh View` | Refresh the tree view (`F5`) |

---

## ⚙️ Configuration

Add to your workspace `.vscode/settings.json`:

```json
{
    "bcuTestGenerator.backgroundValidation": true,
    "bcuTestGenerator.debugMode": false,
    "bcuTestGenerator.maxFileSize": 1048576
}
```

| Setting | Default | Description |
|---------|---------|-------------|
| `backgroundValidation` | `true` | Continuous BCU project validation |
| `debugMode` | `false` | Enable verbose output logging |
| `maxFileSize` | `1048576` | Max file size (bytes) for parsing |

---

## 🔄 Changelog

### v1.6.0 — June 23, 2026
- **New:** Lightweight usage tracking — faster startup, lower memory footprint
- **New:** Cyclomatic complexity analysis for smarter test prioritization
- **Improved:** Reduced 3,308 lines of analytics overhead
- **Improved:** Reduced network dependency (fully functional offline)

### v1.5.0 — November 5, 2025
- **New:** Multi-scenario BCU test report support (cfg2, cfg3, maxcfg, etc.)
- **New:** Automatic scenario detection from file naming patterns
- **New:** Interactive scenario tabs in Results dashboard
- **New:** ZIP archive support for packaged multi-scenario reports
- **Improved:** Aggregated statistics across all scenarios

See [RELEASE_NOTES.md](./RELEASE_NOTES.md) for full release details.

---

## 🤝 Support

- **Issues / Requests:** [GitHub Issues](https://github.boschdevcloud.com/ANN5COB/bcu-test-generator-pro/issues)
- **Installation Help:** See [INSTALLATION_GUIDE.md](./INSTALLATION_GUIDE.md)
- **Author:** Andrew Nelson (MS/ESS12-PS) — Bosch Global Software Technologies

---

*Version 1.7.0 | Released August 10, 2026 | License: BGSW*
