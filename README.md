# VSCode Settings

***[汉语](README.zh.md)***

Personal Visual Studio Code configuration file with customized preferences for formatting, editor behavior, and development workflows.

## 🔎 Overview

This repository contains a carefully crafted Visual Studio Code settings configuration designed to enhance productivity and provide a consistent development experience across different programming languages and frameworks.

## ✨ Features

- **Multi-language formatting support** - Configured formatters for various file types
- **Enhanced editor experience** - Smooth scrolling, cursor animations, and optimized UI
- **Intelligent code actions** - Auto-fix, import organization, and code cleanup on save  
- **Git integration** - Streamlined version control workflow
- **Terminal customization** - Multiple shell profiles with conda integration
- **Extension optimization** - Telemetry disabled and performance-focused settings
- **Developer-friendly defaults** - Reduced confirmation dialogs and smart suggestions

## 🚀 Usage

### Quick Setup

1. Backup your existing VSCode settings (if any)
2. Copy the `settings.json` content to your VSCode user settings
3. Install recommended extensions for optimal experience
4. Restart VSCode to apply all changes

### Accessing VSCode Settings

- **Windows/Linux**: `Ctrl + ,` or File → Preferences → Settings
- **macOS**: `Cmd + ,` or Code → Preferences → Settings
- Click the "Open Settings (JSON)" icon in the top-right corner

## 🔧 Configuration Highlights

This configuration includes optimizations for:

- **Language Support**: JavaScript, TypeScript, Python, HTML, CSS, Markdown, Docker, YAML, and more
- **Code Quality**: Integrated linting, formatting, and auto-fixing
- **Performance**: Optimized computation limits and smooth animations
- **Accessibility**: Unicode support for Chinese characters and multiple locales
- **Privacy**: Telemetry disabled across multiple extensions

## 📋 Prerequisites

### Required Extensions

For the best experience, install these extensions:

- **Prettier**: `esbenp.prettier-vscode`
- **Ruff**: `charliermarsh.ruff` (Python formatting/linting)
- **Markdown Lint**: `DavidAnson.vscode-markdownlint`
- **XML Tools**: `redhat.vscode-xml`
- **Docker**: `ms-azuretools.vscode-containers`
- **Material Icon Theme**: `PKief.material-icon-theme`

### Optional but Recommended

- **GitHub Copilot**: `GitHub.copilot`
- **GitLens**: `eamodio.gitlens`
- **Markdown Preview Enhanced**: `shd101wyy.markdown-preview-enhanced`

### AI Development Tools

- **[Claude Code](https://github.com/anthropic-ai/claude-code)**: Advanced AI-powered coding assistant
  - **Installation & Management**: Use the comprehensive [Claude Code Toolkit](https://github.com/xixu-me/Claude-Code-Toolkit) for easy installation and multi-provider management
  - **Features**: Context-aware code generation, debugging assistance, and refactoring support
  - **Multi-Provider Support**: Switch between Anthropic API, Moonshot AI (latest Kimi models), and custom providers
  - **Cross-Platform**: Works on Linux/macOS (Bash) and Windows (PowerShell)

- **[Gemini CLI](https://github.com/google-gemini/gemini-cli)**: Google's official command-line AI workflow tool
  - **Installation**: `npm install -g @google/gemini-cli` or `npx @google/gemini-cli`
  - **Features**: 1M+ token context window, multimodal capabilities, built-in tools for file system and shell operations
  - **Integration**: MCP server support, VS Code companion extension, sandboxed execution environment
  - **Authentication**: Supports Google API keys, Vertex AI, and Google Workspace accounts

## 📦 Installation

### Method 1: Direct Copy

```bash
# Navigate to your VSCode settings directory
# Windows: %APPDATA%\Code\User\
# macOS: ~/Library/Application Support/Code/User/
# Linux: ~/.config/Code/User/

# Backup existing settings
cp settings.json settings.json.backup

# Copy new settings
curl -o settings.json https://raw.githubusercontent.com/xixu-me/VSCode-Settings/main/settings.json
```

### Method 2: Manual Installation

1. Download the `settings.json` file from this repository
2. Open VSCode Settings (JSON)
3. Replace the content with the downloaded configuration
4. Save the file

## 🎨 Customization

Feel free to modify the configuration according to your needs:

- **Font Settings**: Update `editor.fontFamily` and `editor.fontLigatures`
  
  **About Monaspace Fonts**: This configuration uses [**Monaspace Neon**](https://github.com/githubnext/monaspace) as the default font family. Monaspace is a revolutionary monospaced type superfamily developed by GitHub Next in collaboration with Lettermatic. It consists of five variable axis typefaces (Neon, Argon, Xenon, Radon, and Krypton) that share the same metrics but offer distinct visual personalities.
  
  **Key Features:**
  - **Texture Healing**: Pioneering technology that automatically adjusts character spacing for improved readability
  - **Advanced Ligatures**: Comprehensive coding ligature support with 10 stylistic sets (`ss01`-`ss10`)
  - **Character Variants**: Extensive glyph alternatives using OpenType features (`cv01`-`cv79`)
  - **Nerd Fonts Integration**: Built-in developer icons and symbols
  - **Font Ligatures**: Configured with `'calt', 'liga', 'ss01', 'ss02', 'ss03', 'ss04', 'ss05', 'ss06', 'ss07', 'ss08', 'ss09'` for optimal coding experience

- **Theme**: Change `workbench.colorTheme` and `workbench.iconTheme`
- **Formatters**: Adjust language-specific formatter preferences
- **Terminal**: Modify terminal profiles in `terminal.integrated.profiles.windows`

## 📄 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

**Important Notice**: This configuration is provided as-is and reflects personal preferences and workflows. Please review and test the settings before applying them to your development environment.

### Before Using

- **Backup your existing settings** - Always create a backup of your current VSCode configuration
- **Review the configuration** - Examine settings that may affect your workflow
- **Test incrementally** - Consider applying sections gradually rather than all at once
- **Extension compatibility** - Ensure you have the required extensions installed

### Potential Considerations

- Some settings may override your existing preferences
- Path configurations might need adjustment for your system
- Certain extensions may require separate installation
- Terminal profiles are configured for Windows with conda
