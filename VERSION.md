# BCU Test Generator Professional - Version Information

## Current Version: 1.5.0
**Release Date**: November 5, 2025  
**License**: BGSW (Bosch Global Software Technologies)

## Version History

### v1.5.0 - November 5, 2025
**🎉 Multi-Scenario BCU Test Report Support**

**Major Features:**
- **NEW**: Comprehensive multi-scenario test report support
- **NEW**: Automatic detection of multiple BCU scenarios (cfg2, cfg3, maxcfg, etc.)
- **NEW**: Interactive scenario tabs in Results dashboard
- **NEW**: Aggregated statistics across all scenarios
- **NEW**: Per-scenario report links (HTML, coverage, folders)
- **NEW**: ZIP archive support for packaged multi-scenario reports
- **NEW**: Support for reports in BCU project root folder

**Enhanced Features:**
- Pattern-based scenario detection from file naming
- Scenario count badge showing total detected scenarios
- Dynamic report link generation per scenario
- Full backward compatibility with single-scenario projects
- Professional UI with scenario tabs and smooth animations

**Technical Implementation:**
- Added `_discoverAllScenarioReports()` method (~100 lines)
- Added `_aggregateScenarioResults()` method (~80 lines)
- Added `_parseLegacySingleScenario()` for backward compatibility (~150 lines)
- Enhanced frontend with ~300 lines of JavaScript
- Added ~150 lines of CSS for scenario UI components

**Package Information:**
- File: `bcu-test-generator-pro.vsix`
- Size: ~395KB
- Files: 109 files (optimized packaging)
- Compatibility: VS Code 1.74.0+

### v1.2.0 - September 20, 2025
**🔧 Major Stability Fixes**
- **FIXED**: Extension deactivation crashes caused by workspace modifications
- **FIXED**: Extension restart cycles after BCU project selection
- **IMPROVED**: Source detection now works without workspace changes
- **ENHANCED**: Added comprehensive debug logging for troubleshooting
- **OPTIMIZED**: Extension stays active throughout entire workflow

**Technical Changes:**
- Disabled `workspace.updateWorkspaceFolders()` calls that triggered crashes
- Implemented `detectSourceFilesWithoutWorkspaceModification` method
- Added verification markers for fix deployment confirmation
- All BCU project functionality preserved without workspace modifications

**Package Information:**
- File: `bcu-test-generator-pro.vsix`
- Size: ~292KB
- Compatibility: VS Code 1.74.0+

### v1.1.0 - September 18, 2025
- Enhanced BCU project detection
- Improved source file analysis
- Added analytics tracking

### v1.0.0 - September 5, 2025
- Initial release
- Basic BCU project management
- Test case generation capabilities

## Installation
Download the latest `bcu-test-generator-pro.vsix` and install via VS Code Extensions.

## License
Copyright (c) 2025 Bosch Global Software Technologies (BGSW)
All rights reserved. Internal use only.

---
*For support and updates, contact the BCU Tools development team.*