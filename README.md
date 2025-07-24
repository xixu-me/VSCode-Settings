# VS Code Settings

***[汉语](README.zh.md)***

Personal Visual Studio Code configuration file with customized preferences for formatting, editor behavior, and development workflows. This configuration is compatible with all [Code-OSS](https://github.com/microsoft/vscode)-based editors (VS Code, Trae, Kiro, etc.) and can be shared across multiple editors using symbolic links.

## 🔎 Overview

This repository contains a carefully crafted Visual Studio Code settings configuration designed to enhance productivity and provide a consistent development experience across different programming languages and frameworks.

**Cross-Editor Compatibility**: The `settings.json` file is fully compatible with all Code-OSS-based editors including:

- Visual Studio Code
- Trae
- Kiro
- Lingma
- Other VS Code-compatible editors

**Shared Configuration**: You can use symbolic links to share the same configuration across multiple Code-OSS-based editors, ensuring consistent settings and workflows across your development environment.

## ✨ Features

- **Multi-language formatting support** - Configured formatters for various file types
- **Enhanced editor experience** - Smooth scrolling, cursor animations, and optimized UI
- **Intelligent code actions** - Auto-fix, import organization, and code cleanup on save  
- **Git integration** - Streamlined version control workflow
- **Terminal customization** - Multiple shell profiles with conda integration
- **Extension optimization** - Telemetry disabled and performance-focused settings
- **Developer-friendly defaults** - Reduced confirmation dialogs and smart suggestions

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

- **[Qwen Code](https://github.com/QwenLM/qwen-code)**: Command-line AI workflow tool optimized for Qwen3-Coder models
  - **Installation**: `npm install -g @qwen-code/qwen-code`
  - **Features**: Enhanced parser for Qwen-Coder models, large codebase understanding, workflow automation
  - **Code Capabilities**: Query and edit beyond context limits, automate pull requests and complex rebases
  - **Configuration**: OpenAI-compatible API support with custom base URLs and models

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
# Navigate to VS Code settings directory
# Windows: %APPDATA%\Code\User\
# macOS: ~/Library/Application Support/Code/User/
# Linux: ~/.config/Code/User/

cp settings.json settings.json.backup  # Backup existing settings
curl -o settings.json https://raw.githubusercontent.com/xixu-me/VSCode-Settings/main/settings.json
```

### Method 2: Manual Installation

1. Download `settings.json` from this repository
2. Open VS Code Settings (JSON): `Ctrl/Cmd + ,` → "Open Settings (JSON)" icon
3. Replace content with the downloaded configuration

### Method 3: Symbolic Links (Cross-Editor Sharing)

To share the same configuration across multiple Code-OSS-based editors:

**Linux:**

```bash
# Example: Link Trae and Kiro to use the same settings as VS Code
ln -s "~/.config/Code/User/settings.json" "~/.config/Trae/User/settings.json"
ln -s "~/.config/Code/User/settings.json" "~/.config/Kiro/User/settings.json"
```

**macOS:**

```bash
# Example: Link Trae and Kiro to use the same settings as VS Code
ln -s "~/Library/Application Support/Code/User/settings.json" "~/Library/Application Support/Trae/User/settings.json"
ln -s "~/Library/Application Support/Code/User/settings.json" "~/Library/Application Support/Kiro/User/settings.json"
```

**Windows (PowerShell):**

```powershell
# Example: Link Trae and Kiro to use the same settings as VS Code
New-Item -ItemType SymbolicLink -Path "$env:APPDATA\Trae\User\settings.json" -Target "$env:APPDATA\Code\User\settings.json"
New-Item -ItemType SymbolicLink -Path "$env:APPDATA\Kiro\User\settings.json" -Target "$env:APPDATA\Code\User\settings.json"
```

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
- **Formatters**: Adjust language-specific formatter preferences and auto-formatting behavior
  - **Multi-Language Support**: Pre-configured formatters for CSS, HTML, JavaScript, TypeScript, Python, Markdown, YAML, XML, and more
  - **Format-on-Save**: Automatic code formatting when saving files (`editor.formatOnSave: true`)
  - **Format-on-Type**: Real-time formatting as you type (`editor.formatOnType: true`)
  - **Code Actions**: Auto-fix imports, organize code, and apply linting rules on save
- **Terminal**: Modify terminal profiles in `terminal.integrated.profiles.windows`

## 📄 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

**Important**: This configuration reflects personal preferences. Please backup your existing settings and review the configuration before applying.

**Considerations**: Some settings may override your preferences, paths might need adjustment for your system, and terminal profiles are configured for Windows with conda.

---

Made with ❤️ for the developer community
