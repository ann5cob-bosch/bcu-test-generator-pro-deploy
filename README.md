# BCU Test Generator Professional

<div align="center">

![BCU Test Generator Pro Logo](https://img.shields.io/badge/BCU-Test%20Generator%20Pro-blue?style=for-the-badge&logo=visual-studio-code)

**Next-generation BCU project management and AI-powered test case generation toolkit for Visual Studio Code**

[![Version](https://img.shields.io/badge/version-1.6.0-blue.svg)](https://github.boschdevcloud.com/ANN5COB/bcu-test-generator-pro)
[![License](https://img.shields.io/badge/license-BGSW-green.svg)](LICENSE)
[![VS Code](https://img.shields.io/badge/VS%20Code-1.74.0%2B-brightgreen.svg)](https://code.visualstudio.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-4.9%2B-blue.svg)](https://www.typescriptlang.org/)

[📋 Features](#-features) • [🚀 Quick Start](#-quick-start) • [📖 Documentation](#-documentation) • [🛠️ Development](#%EF%B8%8F-development) • [📊 Analytics](#-analytics)

---

### 🎯 Transform your BCU testing workflow with AI-powered automation

</div>

## 📋 Features

### 🧠 **AI-Powered Test Generation**
- **Advanced LLM Integration**: Seamless GitHub Copilot integration with BCU-specific prompts
- **Template-Driven Generation**: Production-ready test cases using verified BCU 2.5.1 patterns
- **2-Step Workflow**: Streamlined Analysis → Implementation process for maximum efficiency
- **Progressive Complexity**: Level 1 → Level 4 test implementation with increasing sophistication

### 🎯 **Smart C Function Analysis**
- **Enhanced Detection**: Advanced regex parsing with AUTOSAR compliance and macro filtering
- **Function Pointers**: Support for complex function types and callback mechanisms
- **Background Scanning**: Intelligent file-by-file processing with safety constraints
- **Performance Optimized**: Eligibility filtering and size limits for large codebases

### 🎮 **Professional Dashboard Interface**
- **Modern WebView**: Card-based layout with smooth animations and responsive design
- **Multi-Tab Layout**: Project overview, execution monitoring, results analysis, and review management
- **Real-Time Progress**: Live execution tracking with detailed progress visualization
- **Dark/Light Themes**: Professional styling that adapts to VS Code themes

### ⚡ **Advanced Execution Management**
- **Smart Toggle Controls**: Modern switch interface for BCU command parameters
  - 🔧 **Function Mocking** (`-calltrace`): Enable/disable call tracing
  - 📊 **Code Coverage** (`-ctc`): Toggle coverage analysis  
  - 🚫 **No DSM Library** (`-nodsm`): Exclude DSM library usage
  - 📦 **Archive Results**: Automatic result packaging
- **Multiple Execution Modes**:
  - 🔄 **Execute All**: Run all test cases with locked optimal settings
  - 🎯 **Execute Selected**: Choose specific test cases with customizable options
  - 🔧 **Execute Function**: Run tests for individual functions

### 🔍 **Intelligent Project Management**
- **Automatic Discovery**: Smart detection of `.bcuproj` files and project validation
- **Background Validation**: Continuous monitoring with performance optimization
- **Source Detection**: Automatic C source file discovery with workspace integration
- **File Watching**: Real-time updates on project file changes

### 📊 **Lightweight Usage Tracking**
- **Efficient Tracking**: Fast and lightweight usage analytics with minimal overhead
- **Essential Metrics**: Extension activation, test execution, and test generation tracking
- **Reduced Complexity**: Simplified codebase with 3,308 lines of code removed
- **Privacy Focused**: Optional network connectivity with graceful fallback

## 🚀 Quick Start

### Prerequisites (For Users)
- **Visual Studio Code** 1.74.0 or higher
- **BCU Framework** installed and accessible in your environment
- **Workspace** containing `.bcuproj` files
- **Node.js NOT required** - Extension is pre-compiled and ready to use

### Prerequisites (For Developers)
- **Visual Studio Code** 1.74.0 or higher
- **Node.js** 16.x or higher (for building from source)
- **Git** (optional, for version control)

### Installation

#### Method 1: Manual Installation (Current)
1. Download the latest [bcu-test-generator-pro.vsix](./bcu-test-generator-pro.vsix)
2. Open VS Code → Extensions (Ctrl+Shift+X)
3. Click "..." menu → "Install from VSIX..."
4. Select the downloaded `.vsix` file
5. Reload VS Code when prompted

#### Method 2: Command Line Installation
```bash
# Navigate to the extension directory
cd /path/to/BCUTestGenTool_VSCodeExtn

# Install the extension
code --install-extension ./bcu-test-generator-pro.vsix
```

### First Steps

1. **Open BCU Project**
   ```
   📁 Open workspace containing .bcuproj files
   🚀 Click the rocket icon in Activity Bar
   📋 Use "Browse BCU Project" to select your project
   ```

2. **Automatic Setup**
   ```
   ✅ Extension validates project structure
   🔍 Automatically detects source files
   📊 Scans and parses C functions
   🎯 Ready for test generation
   ```

3. **Generate Tests**
   ```
   🎯 Select function from the dashboard
   🧠 Click "Generate AI Test Cases"
   📝 Review generated templates
   ▶️ Execute tests with smart controls
   ```

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

## � Documentation

### Core Concepts

#### BCU Project Structure
```
your-bcu-project/
├── � your_project.bcuproj        # BCU project file (required)
├── 📁 src/                        # Source files
│   ├── 📄 module1.c
│   ├── 📄 module1.h
│   └── 📄 ...
├── 📁 My/                         # BCU test directory
│   ├── 📄 my_your_project_ut.c    # Generated unit tests
│   ├── � stub_functions.c        # Generated stubs
│   └── 📄 ...
└── 📁 BCU_Out/                    # BCU output directory
    ├── 📄 test_results.log
    └── 📄 ...
```

#### Template System
The extension uses a modern 2-step template system:

1. **Analysis & Preparation** (`BCU_Step1_Analysis.md`)
   - Function signature and behavior analysis
   - Dependency classification and mapping
   - Infrastructure assessment and planning
   - Test scenario identification

2. **Test Implementation** (`BCU_Step2_Implementation.md`)
   - Production-ready BCU test code generation
   - Stub and helper function creation
   - Configuration-based test scenarios
   - Proper BCU 2.5.1 compliance

#### AI Integration Workflow
```mermaid
graph LR
    A[Select Function] --> B[Load Template]
    B --> C[Generate Prompt]
    C --> D[Copilot Analysis]
    D --> E[Review & Refine]
    E --> F[Execute Tests]
```

### Commands Reference

| Command | Description | Shortcut |
|---------|-------------|----------|
| `BCU Pro: Open Dashboard` | Launch the main interface | `Ctrl+Shift+P` → BCU |
| `BCU Pro: Browse BCU Project` | Select and validate project | Activity Bar 🚀 |
| `BCU Pro: Generate AI Test Cases` | Create tests for selected function | Dashboard |
| `BCU Pro: Execute All Test Cases` | Run complete test suite | Dashboard |
| `BCU Pro: Detect Source Files` | Scan for C source files | Auto/Manual |
| `BCU Pro: Refresh View` | Update project state | `F5` in tree view |

### Configuration

The extension supports workspace-level configuration:

```json
{
    "bcuTestGenerator.analytics.enabled": true,
    "bcuTestGenerator.backgroundValidation": true,
    "bcuTestGenerator.debugMode": false,
    "bcuTestGenerator.templatePath": "./templates",
    "bcuTestGenerator.maxFileSize": 1048576
}
```

## 🛠️ Development

### Building from Source

1. **Clone Repository**
   ```bash
   git clone https://github.com/ann5cob-bosch/BCU_TestCaseGenerator_Pro.git
   cd BCU_TestCaseGenerator_Pro
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Compile TypeScript**
   ```bash
   # Production build
   npm run compile
   
   # Development with watch mode
   npm run watch
   ```

4. **Package Extension**
   ```bash
   # Create .vsix package
   vsce package
   ```

### Project Structure

```
BCUTestGenTool_VSCodeExtn/
├── 📁 src/                         # TypeScript source code
│   ├── 📄 extension.ts             # Main extension provider (7,155 lines)
│   ├── 📄 webviewProvider.ts       # Dashboard interface (4,199 lines)
│   └── 📄 analyticsTracker.ts      # Analytics system (2,283 lines)
├── 📁 templates/                   # AI generation templates
│   ├── 📄 BCU_Step1_Analysis.md    # Analysis template
│   ├── 📄 BCU_Step2_Implementation.md # Implementation template
│   ├── 📄 BCU_Workflow_Guide.md    # User workflow guide
│   └── 📄 BCU_Quick_Generation_Prompt.md # Quick generation
├── � media/                       # WebView assets
│   ├── 📄 dashboard.html           # Main dashboard UI
│   ├── 📄 dashboard.css            # Professional styling
│   └── 📄 dashboard.js             # Interactive functionality
├── 📁 scripts/                     # Automation scripts
│   ├── 📄 analytics_powerbi_parser.py # Analytics processing
│   └── 📄 run_analytics_parser.bat # Batch automation
├── 📄 package.json                 # Extension manifest
├── 📄 tsconfig.json               # TypeScript configuration
└── 📄 CHANGELOG.md                # Version history
```

### Key Architecture Components

#### Extension Provider (`src/extension.ts`)
- **BcuTestGeneratorProvider**: Main class implementing TreeDataProvider
- **Background Processing**: Validation, scanning, and file watching
- **Function Analysis**: Advanced C parsing with AUTOSAR support
- **Test Execution**: BCU command integration with progress monitoring

#### WebView Provider (`src/webviewProvider.ts`)
- **Modern Dashboard**: Professional web-based interface
- **Real-time Updates**: Live execution monitoring and progress tracking
- **Message Handling**: Bidirectional communication with VS Code
- **State Management**: Persistent UI state and user preferences

#### Usage Tracker (`src/usageTracker.ts`)
- **Lightweight Tracking**: Fast and efficient usage recording
- **Essential Metrics**: Extension activation, test execution, and generation tracking
- **Graceful Fallback**: Optional network connectivity with offline support
- **Performance Optimized**: Minimal memory footprint and startup impact

#### Complexity Analysis (`src/cyclomaticComplexity.ts`)
- **McCabe Complexity**: Computes cyclomatic complexity for C functions
- **Test Coverage Planning**: Analyzes boolean operators for conditional paths
- **Smarter Generation**: Enables better test case prioritization

### Development Guidelines

#### Code Style
- **TypeScript**: Strict type checking with comprehensive interfaces
- **Async/Await**: Modern asynchronous programming patterns
- **Error Handling**: Enterprise-grade error catching and user feedback
- **Documentation**: Comprehensive JSDoc comments for all public methods

#### Testing Strategy
- **Manual Testing**: Comprehensive workflow testing with real BCU projects
- **Integration Testing**: End-to-end validation with BCU framework
- **Performance Testing**: Large codebase validation and memory monitoring
- **Analytics Validation**: Usage tracking accuracy and privacy compliance

## 📊 Usage Tracking

### Lightweight Tracking System
The extension includes a simplified usage tracking system optimized for performance:

- **Minimal Overhead**: Fast tracking with negligible performance impact
- **Essential Metrics**: Records extension activation, test execution, and test generation
- **Optional Network**: Connection testing is optional and gracefully degrades offline
- **Privacy Focused**: No sensitive data collection or storage

### Complexity Analysis
New in v1.6.0: Cyclomatic complexity analysis for smarter test generation:

- **McCabe Complexity**: Automatic computation of function complexity metrics
- **Conditional Path Mapping**: Analyzes boolean operators for better coverage planning
- **Test Prioritization**: Enables intelligent test case ordering based on complexity
- **Performance Insights**: Helps identify high-risk functions requiring more test coverage
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
*Last updated: June 23, 2026 | Version: 1.6.0*
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

### **Prerequisites (For Regular Users)**
- ✅ Visual Studio Code 1.74.0+
- ✅ BCU project with `.bcuproj` files
- ✅ C source files for analysis
- ❌ **Node.js NOT required** - Extension is pre-compiled

### **Prerequisites (For Developers Only)**
- ✅ Visual Studio Code 1.74.0+
- ✅ Node.js and npm installed (for building from source)
- ✅ TypeScript development environment

### **Installation (For Regular Users)**
1. Install the VSIX file:
   - Method 1: `Ctrl+Shift+P` → "Extensions: Install from VSIX..."
   - Method 2: Command line: `code --install-extension bcu-test-generator-pro-1.5.0.vsix`
2. Reload VS Code
3. Ready to use!

### **Installation (For Developers Only)**
1. Clone or download the extension source code
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
## 🤝 Contributing

We welcome contributions from the automotive software community!

### Getting Started
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Environment
- **Node.js** 16.x or higher
- **TypeScript** 4.9+ for strict type checking
- **VS Code** with recommended extensions
- **BCU Framework** for testing integration

### Code Review Process
- All changes require peer review
- Automated TypeScript compilation validation
- Manual testing with real BCU projects
- Analytics impact assessment

## 📄 License

This project is licensed under the **Bosch Global Software Technologies (BGSW)** License.

**Copyright © 2025 Bosch Global Software Technologies**

## 🙏 Acknowledgments

- **BCU Framework Team** for the excellent unit testing framework
- **Visual Studio Code Team** for the extensible platform
- **GitHub Copilot Team** for AI integration capabilities
- **Bosch Automotive Software Engineers** for feedback and validation

## 📞 Support

### Technical Support
- **Internal Support**: Contact MS/ESS-PS department
- **GitHub Issues**: [Create an issue](https://github.com/ann5cob-bosch/BCU_TestCaseGenerator_Pro/issues)
- **Documentation**: See [templates/README.md](./templates/README.md) for detailed guides

### Enterprise Support
- **Deployment Assistance**: Contact Bosch Global Software Technologies
- **Custom Analytics**: PowerBI integration setup and configuration
- **Training Programs**: Team onboarding and best practices workshops

### Troubleshooting

#### Common Issues
1. **Extension not loading**: Ensure VS Code version 1.74.0+
2. **BCU project not detected**: Verify `.bcuproj` file exists in workspace
3. **Functions not parsing**: Check C source file syntax and encoding
4. **Analytics not working**: Verify network permissions for shared folder access

#### Debug Mode
Enable debug logging in VS Code settings:
```json
{
    "bcuTestGenerator.debugMode": true
}
```

---

<div align="center">

**Built with ❤️ by Bosch Global Software Technologies**

*Empowering automotive software engineers with next-generation testing tools*

![Bosch Logo](https://img.shields.io/badge/Powered%20by-Bosch-red?style=flat-square)
![BCU Framework](https://img.shields.io/badge/BCU-Framework-blue?style=flat-square)
![AI Powered](https://img.shields.io/badge/AI-Powered-green?style=flat-square)

**Version 1.5.0** | **November 2025** | **Enterprise Ready**

</div>
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

### For Regular Users (Installing the Extension)

✅ **No Prerequisites Required** - The extension is pre-compiled and ready to use. Node.js is NOT needed!

**Installation Steps:**

1. **Download the Extension**
   - Get the `bcu-test-generator-pro-1.5.0.vsix` file

2. **Install in VS Code**
   - Method 1: Via UI
     - Open VS Code
     - Press `Ctrl+Shift+P`
     - Type "Extensions: Install from VSIX..."
     - Select the VSIX file
   
   - Method 2: Via Command Line
     ```bash
     code --install-extension bcu-test-generator-pro-1.5.0.vsix
     ```

3. **Reload VS Code**
   - The extension is now ready to use!

### For Developers (Building from Source)

⚠️ **Prerequisites**: Node.js and npm are required ONLY for development.

**Installation Steps:**

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
