# BCU Test Generator Professional v1.0.0

> **Next-generation BCU project management and AI-powered test case generation toolkit for Visual Studio Code**

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/bcu-tools/bcu-test-generator-pro)
[![License](https://img.shields.io/badge/license-Bosch%20Global%20Software%20Technologies-green.svg)](LICENSE)
[![VS Code](https://img.shields.io/badge/VS%20Code-1.74.0%2B-brightgreen.svg)](https://code.visualstudio.com/)

## 🚀 Quick Installation

### Download and Install
1. **Download**: [bcu-test-generator-pro-1.0.0.vsix](./bcu-test-generator-pro-1.0.0.vsix) (338KB)
2. **Install**: Open VS Code → Extensions → "..." → Install from VSIX
3. **Reload**: Restart VS Code when prompted
4. **Access**: Click the rocket icon 🚀 in the Activity Bar

### 📋 Prerequisites
- Visual Studio Code 1.74.0+
- BCU Framework installed and accessible
- Workspace with `.bcuproj` files

## ✨ Key Features

### �️ **Smart Execution Controls**
- **Toggle Button Interface**: Control BCU command parameters with modern switches
  - 🔧 **Function Mocking** (`-calltrace`): Enable/disable call tracing
  - 📊 **Code Coverage** (`-ctc`): Toggle coverage analysis
  - 🚫 **No DSM Library** (`-nodsm`): Exclude DSM library usage
  - 📦 **Archive** (zip): Automatic result archiving
- **Execution Mode Behavior**: Smart toggle states based on execution mode
- **State Persistence**: Settings saved across VS Code sessions

### 🔍 **Enhanced Function Detection**
- **Safer Regex Parsing**: Comprehensive pattern recognition for C functions
- **AUTOSAR Support**: Detection of AUTOSAR-style function declarations
- **Function Pointers**: Advanced parsing for complex function types
- **Background Scanning**: Incremental file-by-file processing with safety limits
- **Performance Optimized**: Intelligent eligibility filtering and size constraints

### 📊 **Modern Dashboard Interface**
- **Multi-Tab Layout**: Project overview, execution, results, and review tabs
- **Real-Time Progress**: Live execution tracking with detailed progress bars
- **Interactive Elements**: Modern UI components with smooth animations
- **Responsive Design**: Adapts to different screen sizes and themes

### ⚡ **Execution Management**
- **Multiple Execution Modes**:
  - 🔄 **Execute All**: Run all test cases with locked optimal settings
  - 🎯 **Execute Selected**: Choose specific test cases with customizable options
  - 🔧 **Execute Function**: Run tests for individual functions
- **Progress Tracking**: Real-time execution monitoring with stage indicators
- **Result Integration**: Seamless BCU report parsing and display

### 🤖 **AI-Powered Test Generation**
- **Python Integration**: Advanced test case generation capabilities
- **Template System**: Customizable prompt templates for AI assistance
- **Workflow Automation**: Streamlined test case creation process

### 📁 **Project Management**
- **BCU Project Detection**: Automatic `.bcuproj` file discovery
- **Source File Analysis**: Intelligent C/C++ source file parsing
- **Test Case Linking**: Automatic function-to-test-case associations
- **Review System**: Track test case review status and progress

## 🏢 Enterprise Features

### 🔒 **Security & Compliance**
- **Bosch Global Software Technologies** licensed
- **Enterprise-grade** security considerations
- **Audit Trail**: Comprehensive logging and tracking

### � **Integration Capabilities**
- **BCU Framework**: Full integration with Build Configuration Utility
- **Coverage Tools**: Support for code coverage analysis
- **CI/CD Ready**: Suitable for automated testing pipelines

### 📈 **Performance & Scalability**
- **Large Project Support**: Optimized for enterprise-scale codebases
- **Memory Efficient**: Smart resource management and cleanup
- **Background Processing**: Non-blocking operations for better UX

## 📚 Documentation

### 📖 **Available Guides**
- 📋 **[Installation Guide](INSTALLATION_GUIDE.md)**: Complete setup instructions with troubleshooting
- 📝 **[Changelog](CHANGELOG.md)**: Version history and feature updates
- ⚙️ **[Git Setup Instructions](GIT_SETUP_INSTRUCTIONS.md)**: Repository configuration guide

### 🎯 **Quick Start**
1. Open workspace with BCU projects
2. Click BCU Test Generator icon (🚀) in Activity Bar
3. Open dashboard for project overview
4. Configure execution options with toggle buttons
5. Execute tests with real-time monitoring

## 🛠️ Technical Specifications

### � **Package Information**
- **Extension Name**: BCU Test Generator Professional
- **Package Size**: 338.02KB
- **File Count**: 52 files
- **Supported Platforms**: Windows, Linux, macOS

### 🔧 **Technology Stack**
- **Frontend**: TypeScript, HTML5, CSS3, JavaScript
- **Backend**: VS Code Extension API, Node.js
- **Integration**: Python, BCU Framework, XML/CSV parsing
- **UI Framework**: Custom webview with modern design patterns

### 📊 **Supported File Types**
- `.bcuproj` - BCU project files
- `.c/.h` - C source and header files
- `.xml` - Test result summaries
- `.csv` - Coverage analysis reports
- `.html` - BCU execution reports

## 🤝 Support & Contact

### � **Getting Help**
- **Issues**: [GitHub Issues](https://github.com/bcu-tools/bcu-test-generator-pro/issues)
- **Documentation**: See installation guide for detailed setup
- **Updates**: Check VS Code Extensions for latest versions

### 👥 **Team**
- **Author**: Andrew Nelson (MS/ESS12-PS)
- **Department**: MS/ESS-PS
- **Organization**: Bosch Global Software Technologies

## 📄 **License & Legal**
- **License**: Bosch Global Software Technologies
- **Copyright**: © 2025 Bosch Global Software Technologies
- **Compliance**: Enterprise-grade security and licensing

---

## 🎉 **Ready for Production Use**

This extension is production-ready and has been thoroughly tested for enterprise deployment. It provides a comprehensive solution for BCU project management with modern UI/UX and advanced automation capabilities.

**Download now and transform your BCU testing workflow!** 🚀

---
*Last updated: September 5, 2025 | Version: 1.0.0*
│   │   └── ⚙️ Dsmad_Clear
│   ├── 🤖 Generate Test Cases for Dsmad_Init
│   └── 🧠 AI Assistant Ready
├── ─────────────────────
└── 🌟 BCU Test Gen Pro v1.0 | Active
```

### **🎨 Color-Coded Status System**
- 🟢 **Green**: Valid, Ready, Success states
- 🔵 **Blue**: Information, Configuration, Analysis
- 🟡 **Yellow**: Selected items, Warnings, Attention needed  
- 🟣 **Purple**: AI features, Advanced functions
- 🔴 **Red**: Errors, Invalid states, Missing requirements

### **💡 Smart Notifications**
- `🚀 Success! BCU project "dsmad" loaded and validated. Ready for test operations.`
- `🧬 Source Analysis Complete | Discovered 15 C functions ready for test generation.`
- `🎯 Function Selected | Dsmad_Init is now ready for AI-powered test case generation.`

---

## 🚀 **Getting Started**

### **Prerequisites**
- ✅ Visual Studio Code 1.74.0+
- ✅ Node.js and npm installed
- ✅ BCU project with `.bcuproj` files
- ✅ C source files for analysis

### **Installation**
1. Clone or download the extension
2. Install dependencies: `npm install`
3. Compile: `npm run compile`
4. Press `F5` to launch Extension Development Host

### **Quick Start Workflow**
1. **🎯 Open Panel** - Find the rocket icon in Activity Bar
2. **🔍 Browse BCU Project** - Select your project folder
3. **⚡ Execute Tests** - Run your test suite with one click
4. **🔬 Browse Source Files** - Analyze C functions automatically
5. **🤖 Generate Test Cases** - Create AI-powered test suites

---

## 🛠️ **Advanced Features**

### **🧠 AI Test Generation**
The extension creates sophisticated prompts for AI assistants:

```markdown
🤖 AI Test Generation Request

Based on the instructions in BCU_TestCase_Generation_Prompt.md, 
generate design testcases for the function Dsmad_Init and add it to 
C:/Project/My/my_dsmad_ut.c

Function Details:
- Name: Dsmad_Init
- Source File: dsmad.c
- Line: 45
- Project: dsmad
- Target: C:/Project/My/my_dsmad_ut.c

Please generate comprehensive test cases including:
✅ Normal operation scenarios
✅ Edge cases and boundary conditions  
✅ Error handling and invalid inputs
✅ Performance and stress testing
✅ Integration test scenarios
```

### **📁 Enhanced File Templates**
Auto-generated test files include professional headers:

```c
/*
 * 🧪 BCU Test Suite - dsmad
 * Generated by BCU Test Generator Pro v1.0
 * 
 * ⚡ AI-powered test cases for comprehensive validation
 * 🎯 Target Function: Dsmad_Init
 * 📁 Source: dsmad.c
 * 
 * Test Categories:
 * ✅ Unit Tests
 * ✅ Integration Tests  
 * ✅ Edge Cases
 * ✅ Error Handling
 */
```

---

## 🎯 **Architecture**

### **🏗️ Modern Extension Structure**
```
BCUTestGenTool_VSCodeExtn/
├── 🎨 Enhanced UI Components
│   ├── Futuristic tree view provider
│   ├── Color-coded status system
│   ├── Interactive command palette
│   └── Smart notification system
├── 🧬 Advanced Parsing Engine
│   ├── Recursive C file scanner
│   ├── Function definition extractor
│   ├── File organization system
│   └── Smart filtering logic
├── 🤖 AI Integration Layer
│   ├── Context-aware prompt generation
│   ├── Template discovery system
│   ├── Target file management
│   └── Intelligent navigation
└── ⚡ Modern VS Code Integration
    ├── Command registration system
    ├── Workspace management
    ├── Terminal integration
    └── File system operations
```

---

## 🎪 **Command Palette Integration**

All features accessible via Command Palette (`Ctrl+Shift+P`):
- `🚀 BCU Pro: Open BCU Test Generator Pro`
- `🔍 BCU Pro: Browse BCU Project`
- `🔬 BCU Pro: Browse Source Files`
- `⚡ BCU Pro: Execute Test Suite`
- `🤖 BCU Pro: Generate AI Test Cases`

---

## 🔮 **Future Roadmap**

### **Planned Enhancements**
- 🎨 **Theme Customization**: Custom color schemes and icon packs
- 🔍 **Advanced Search**: Fuzzy function search with filters
- 📈 **Analytics Dashboard**: Test coverage and performance metrics
- 🤖 **AI Models Integration**: Direct integration with popular AI services
- 🔄 **Auto-Refresh**: Real-time source file monitoring
- 📱 **Mobile Support**: VS Code web compatibility

---

## 🤝 **Contributing**

We welcome contributions to make BCU Test Generator Pro even more amazing!

1. 🍴 Fork the repository
2. 🌟 Create a feature branch
3. ✨ Make your enhancements
4. 🧪 Test thoroughly
5. 🚀 Submit a pull request

---

## 📜 **License**

[Your License Here]

---

<div align="center">

### 🚀 **BCU Test Generator Pro** 
*Revolutionizing BCU development workflows with AI-powered automation*

**⚡ Built with modern VS Code APIs | 🎨 Designed for the future**

</div>

## Setup Instructions

⚠️ **Prerequisites**: This extension requires Node.js and npm to be installed.

### Installation Steps

1. **Install Node.js**
   - Download and install Node.js from [https://nodejs.org/](https://nodejs.org/)
   - Verify installation: Open PowerShell and run `node --version` and `npm --version`

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Compile the Extension**
   ```bash
   npm run compile
   ```

4. **Run the Extension**
   - Press `F5` in VS Code to open Extension Development Host
   - The extension will be loaded and ready for testing

## Requirements

- Visual Studio Code 1.74.0 or higher
- BCU project with `.bcuproj` files
- C source files for function parsing
- Template folder with `BCU_TestCase_Generation_Prompt.md`

## Extension Structure

```
BCUTestGenTool_VSCodeExtn/
├── src/
│   └── extension.ts          # Main extension logic
├── package.json              # Extension manifest
├── tsconfig.json            # TypeScript configuration
└── README.md                # This file
```

## Development

### Building the Extension

```bash
# Compile TypeScript
npm run compile

# Watch for changes
npm run watch
```

### Testing

1. Open this project in VS Code
2. Press F5 to launch Extension Development Host
3. Test the extension functionality

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## Author

**Andrew Nelson (MS/ESS12-PS)**  
Department: MS/ESS-PS  
Business Unit: Bosch Global Software Technologies  

## License

BGSW License

Copyright (c) 2025 Bosch Global Software Technologies

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
