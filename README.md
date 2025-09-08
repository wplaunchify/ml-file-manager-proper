# ML File Manager Pro

**Version:** 1.6.18  
**Author:** 1WD LLC  
**Website:** [WPLaunchify.com](https://wplaunchify.com)  
**License:** GPL v2 or later  

## 🚀 Production-Ready WordPress MCP File Manager

ML File Manager Pro is a comprehensive WordPress plugin that provides complete filesystem access through the Model Context Protocol (MCP). It serves as a complete SFTP replacement, enabling AI agents like Claude (Cursor) to perform full file management operations on your WordPress server.

## ✅ **PRODUCTION READY - VERSION 1.6.18**
- **100% Functionality:** All 12 MCP tools working perfectly
- **Enterprise Security:** Robust path validation and API key management
- **Universal Compatibility:** Works with Cursor, Claude Desktop, and any MCP client
- **Comprehensive Documentation:** Ready for deployment and integration

## 📁 Repository Structure

```
ml-file-manager/
├── README.md                    # This file
├── plugin-files/               # Production plugin files
│   └── ml-file-manager.php     # Main plugin file
├── old-versions/               # Version history
│   ├── v1.4.1/                # Initial working version
│   ├── v1.6.0/                # Development versions
│   ├── v1.6.18-FINAL-BACKUP/  # Final backup with changelog
│   └── ...                    # Other versions
└── research/                   # Development research
```

## 📦 Installation

1. Download `plugin-files/ml-file-manager.php`
2. Upload to your `/wp-content/plugins/` directory
3. Activate through WordPress admin
4. Configure API keys in ML File Manager settings

## 🔧 Configuration

### For Cursor IDE (Recommended)

```json
{
  "mcpServers": {
    "ml-file-manager": {
      "command": "npx",
      "args": [
        "-y", "-p", "mcp-remote@0.1.29", "-p", "undici@7",
        "mcp-remote",
        "https://yoursite.com/wp-json/ml-file-manager/v1/mcp-http?X-API-Key=YOUR_API_KEY",
        "--transport", "http-only"
      ]
    }
  }
}
```

## 🛠️ Available MCP Tools (All 12 - 100% Functional)

### Core Operations
- `mcp_ml-file-manager_get_status` - System status
- `mcp_ml-file-manager_list_files` - List files/directories  
- `mcp_ml-file-manager_fs_stat` - File information

### File Operations
- `mcp_ml-file-manager_fs_read` - Read file contents
- `mcp_ml-file-manager_fs_write` - Write file contents
- `mcp_ml-file-manager_fs_delete` - Delete files/directories

### Advanced Operations
- `mcp_ml-file-manager_fs_copy` - Copy files/directories
- `mcp_ml-file-manager_fs_move` - Move/rename files
- `mcp_ml-file-manager_fs_chmod` - Change permissions
- `mcp_ml-file-manager_fs_zip` - Create ZIP archives
- `mcp_ml-file-manager_fs_unzip` - Extract ZIP archives
- `mcp_ml-file-manager_fs_glob` - Find files by pattern

## 🔒 Security Features

- **Path Validation:** Prevents directory traversal attacks
- **API Key Management:** Secure token-based authentication
- **Allowed Roots:** Configurable filesystem access boundaries
- **WordPress Integration:** Native permission system

## 🚀 Production Deployment

### System Requirements
- **WordPress:** 5.0+
- **PHP:** 7.4+
- **Extensions:** ZipArchive (for archive operations)

### Performance
- **File Size Limits:** 2MB read limit
- **Glob Results:** 5000 file limit
- **Memory Optimized:** Efficient operations

## 🔄 Version History

### v1.6.18 (Current - Production Ready) ✅
- **100% Functionality:** All 12 MCP tools working perfectly
- **Final Breakthrough:** Fixed RPC parameter mismatches
- **Production Ready:** Comprehensive testing completed
- **Security Hardened:** Robust path validation

## 🤝 Support

- **Website:** [WPLaunchify.com](https://wplaunchify.com)
- **Documentation:** Available in WordPress admin
- **GitHub:** Issues and feature requests

---

**Developed by 1WD LLC** | **[WPLaunchify.com](https://wplaunchify.com)**

*Empowering WordPress with AI-driven file management capabilities.*