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

## 🚀 使用方法

### 快速设置

1. 备份现有的 VSCode 设置（如果有）
2. 将 `settings.json` 内容复制到您的 VSCode 用户设置中
3. 安装推荐的扩展以获得最佳体验
4. 重启 VSCode 以应用所有更改

### 访问 VSCode 设置

- **Windows/Linux**: `Ctrl + ,` 或文件 → 首选项 → 设置
- **macOS**: `Cmd + ,` 或代码 → 首选项 → 设置
- 点击右上角的"打开设置 (JSON)"图标

## 🔧 配置亮点

此配置包含以下优化：

- **语言支持**: JavaScript、TypeScript、Python、HTML、CSS、Markdown、Docker、YAML 等
- **代码质量**: 集成的代码检查、格式化和自动修复
- **性能**: 优化的计算限制和平滑动画
- **可访问性**: 中文字符和多语言环境的 Unicode 支持
- **隐私**: 在多个扩展中禁用遥测

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

## 📦 安装说明

### 方法一：直接复制

```bash
# 导航到您的 VSCode 设置目录
# Windows: %APPDATA%\Code\User\
# macOS: ~/Library/Application Support/Code/User/
# Linux: ~/.config/Code/User/

# 备份现有设置
cp settings.json settings.json.backup

# 复制新设置
curl -o settings.json https://raw.githubusercontent.com/xixu-me/VSCode-Settings/main/settings.json
```

### 方法二：手动安装

1. 从本仓库下载 `settings.json` 文件
2. 打开 VSCode 设置 (JSON)
3. 用下载的配置替换内容
4. 保存文件

## 🎨 自定义设置

欢迎根据您的需求修改配置：

- **字体设置**: 更新 `editor.fontFamily` 和 `editor.fontLigatures`
- **主题**: 更改 `workbench.colorTheme` 和 `workbench.iconTheme`
- **格式化程序**: 调整特定语言的格式化程序首选项
- **终端**: 修改 `terminal.integrated.profiles.windows` 中的终端配置文件

## 📄 许可证

本项目根据 GNU 通用公共许可证 v3.0 许可 - 有关详细信息，请参见 [LICENSE](LICENSE) 文件。

## ⚠️ 免责声明

**重要提示**: 此配置按原样提供，反映了个人偏好和工作流程。请在将其应用于您的开发环境之前审查和测试设置。

### 使用前请注意

- **备份现有设置** - 始终创建当前 VSCode 配置的备份
- **审查配置** - 检查可能影响您工作流程的设置
- **逐步测试** - 考虑逐渐应用各部分而不是一次性全部应用
- **扩展兼容性** - 确保您已安装所需的扩展

### 潜在考虑因素

- 某些设置可能会覆盖您现有的首选项
- 路径配置可能需要根据您的系统进行调整
- 某些扩展可能需要单独安装
- 终端配置文件是为带有 conda 的 Windows 配置的
