# VSCode 设置

***[English](README.md)***

个人 Visual Studio Code 配置文件，包含用于格式化、编辑器行为和开发工作流的自定义首选项。

## 🔎 概述

本仓库包含精心制作的 Visual Studio Code 设置配置，旨在提高生产力并为不同编程语言和框架提供一致的开发体验。

## ✨ 功能特性

- **多语言格式化支持** - 为各种文件类型配置格式化程序
- **增强编辑器体验** - 平滑滚动、光标动画和优化的用户界面
- **智能代码操作** - 保存时自动修复、导入整理和代码清理
- **Git 集成** - 简化的版本控制工作流
- **终端自定义** - 支持 conda 集成的多种 shell 配置
- **扩展优化** - 禁用遥测和专注性能的设置
- **开发者友好的默认设置** - 减少确认对话框和智能建议

## 📋 前置条件

### 必需扩展

为了获得最佳体验，请安装这些扩展：

- **Prettier**: `esbenp.prettier-vscode`
- **Ruff**: `charliermarsh.ruff` (Python 格式化/代码检查)
- **Markdown Lint**: `DavidAnson.vscode-markdownlint`
- **XML Tools**: `redhat.vscode-xml`
- **Docker**: `ms-azuretools.vscode-containers`
- **Material Icon Theme**: `PKief.material-icon-theme`

### 可选但推荐

- **GitHub Copilot**: `GitHub.copilot`
- **GitLens**: `eamodio.gitlens`
- **Markdown Preview Enhanced**: `shd101wyy.markdown-preview-enhanced`

### AI 开发工具

- **[Claude Code](https://github.com/anthropic-ai/claude-code)**: 先进的 AI 编程助手
  - **安装和管理**: 使用全面的 [Claude Code 工具包](https://github.com/xixu-me/Claude-Code-Toolkit) 轻松安装和管理多提供商
  - **功能特性**: 上下文感知的代码生成、调试辅助和重构支持
  - **多提供商支持**: 在 Anthropic API、月之暗面（最新 Kimi 模型）和自定义提供商之间切换
  - **跨平台**: 适用于 Linux/macOS (Bash) 和 Windows (PowerShell)

- **[Gemini CLI](https://github.com/google-gemini/gemini-cli)**: Google 官方命令行 AI 工作流工具
  - **安装**: `npm install -g @google/gemini-cli` 或 `npx @google/gemini-cli`
  - **功能特性**: 100 万+ 令牌上下文窗口、多模态能力、内置文件系统和 shell 操作工具
  - **集成**: MCP 服务器支持、VS Code 配套扩展、沙盒执行环境
  - **身份验证**: 支持 Google API 密钥、Vertex AI 和 Google Workspace 账户

## 📦 安装说明

### 方法一：直接复制

```bash
# 导航到 VSCode 设置目录
# Windows: %APPDATA%\Code\User\
# macOS: ~/Library/Application Support/Code/User/
# Linux: ~/.config/Code/User/

cp settings.json settings.json.backup  # 备份现有设置
curl -o settings.json https://raw.githubusercontent.com/xixu-me/VSCode-Settings/main/settings.json
```

### 方法二：手动安装

1. 从本仓库下载 `settings.json` 文件
2. 打开 VSCode 设置 (JSON)：`Ctrl/Cmd + ,` → "打开设置 (JSON)"图标
3. 用下载的配置替换内容
4. 保存文件

## 🎨 自定义设置

欢迎根据您的需求修改配置：

- **字体设置**: 更新 `editor.fontFamily` 和 `editor.fontLigatures`
  
  **关于 Monaspace 字体**: 此配置使用 [**Monaspace Neon**](https://github.com/githubnext/monaspace) 作为默认字体系列。Monaspace 是由 GitHub Next 与 Lettermatic 合作开发的革命性等宽字体超家族。它包含五个可变轴字体（Neon、Argon、Xenon、Radon 和 Krypton），具有相同的字符间距但提供不同的视觉特性。
  
  **主要特色:**
  - **文理愈合**: 开创性技术，可自动调整字符间距以提高可读性
  - **高级连字**: 全面的编程连字支持，包含 10 个样式集（`ss01`-`ss10`）
  - **字符变体**: 使用 OpenType 功能提供大量字形替代方案（`cv01`-`cv79`）
  - **Nerd Fonts 集成**: 内置开发者图标和符号
  - **字体连字**: 配置了 `'calt', 'liga', 'ss01', 'ss02', 'ss03', 'ss04', 'ss05', 'ss06', 'ss07', 'ss08', 'ss09'` 以获得最佳编程体验

- **主题**: 更改 `workbench.colorTheme` 和 `workbench.iconTheme`
- **格式化程序**: 调整特定语言的格式化程序首选项和自动格式化行为
  - **多语言支持**: 为 CSS、HTML、JavaScript、TypeScript、Python、Markdown、YAML、XML 等预配置格式化程序
  - **保存时格式化**: 保存文件时自动格式化代码 (`editor.formatOnSave: true`)
  - **输入时格式化**: 键入时实时格式化 (`editor.formatOnType: true`)
  - **代码操作**: 保存时自动修复导入、整理代码和应用代码检查规则
- **终端**: 修改 `terminal.integrated.profiles.windows` 中的终端配置文件

## 📄 许可证

本项目根据 GNU 通用公共许可证 v3.0 许可 - 有关详细信息，请参见 [LICENSE](LICENSE) 文件。

## ⚠️ 免责声明

本配置文件基于个人开发经验设计。使用前请备份现有设置，部分功能需要特定插件或字体支持。建议根据个人需求适当调整。
