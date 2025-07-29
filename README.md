# Magic Claude

> Magic Claude - 专业的 Claude CLI 桌面应用和开发工具包

**由 [Magic666.top](https://magic666.top) 提供技术支持**

Magic666.top 是一个专注于AI技术服务的平台，为开发者和企业提供高质量的 Claude API 代理服务。我们致力于：
- 🚀 提供稳定可靠的 API 服务
- 🔒 保障用户数据安全和隐私
- 💡 不断创新和优化用户体验
- 🌟 构建开放友好的 AI 生态

[![Release](https://img.shields.io/github/v/release/anyme123/magic-claude?color=brightgreen)](https://github.com/anyme123/magic-claude/releases)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Cross--Platform-brightgreen)](https://github.com/anyme123/magic-claude)
[![Magic666](https://img.shields.io/badge/Powered%20by-Magic666.top-purple)](https://magic666.top)

## ✨ 特性

### 🎯 核心功能
- **项目管理**: 可视化管理 Claude 项目，支持会话历史和检查点
- **实时交互**: 流式显示 Claude 响应，支持 Markdown 渲染和语法高亮
- **智能代理**: Agent 系统支持 GitHub 集成和自动化任务执行
- **MCP 支持**: 完整的 Model Context Protocol 服务器管理

### 🔧 Magic666 集成服务
- **官方集成**: 深度集成 Magic666.top API 服务
- **安全可靠**: 由 Magic666.top 提供的稳定 API 服务
- **隐私保护**: 本地存储配置，保护用户隐私
- **即插即用**: 预配置 Magic666.top 服务地址
- **技术支持**: Magic666.top 专业技术团队支持

### 🌟 用户体验
- **多语言支持**: 中文优先的国际化界面
- **主题切换**: 支持明暗主题，使用 OKLCH 色彩空间
- **响应式设计**: 适配不同屏幕尺寸的桌面应用
- **键盘快捷键**: 丰富的快捷键支持，提升操作效率

## 🚀 快速开始

### 系统要求

- **操作系统**: Windows 10/11 (64位)
- **Node.js**: 18.0+ (推荐 LTS 版本)
- **Claude CLI**: 需要预先安装 Claude CLI

### 安装方式

#### 方式一：下载预构建版本 (推荐)
1. 前往 [Releases 页面](https://github.com/anyme123/magic-claude/releases)
2. 下载对应平台的安装包：
   - Windows: `Magic Claude_x.x.x_x64-setup.exe` (NSIS 安装包)
   - Windows: `Magic Claude_x.x.x_x64_en-US.msi` (MSI 安装包)
   - macOS: `Magic Claude_x.x.x_x64.dmg` (DMG 安装包)
3. 运行安装程序并完成安装

#### 方式二：从源代码构建
```bash
# 克隆仓库
git clone https://github.com/anyme123/magic-claude.git
cd magic-claude

# 安装依赖 (推荐使用 Bun)
bun install

# 开发模式运行
bun run tauri dev

# 构建生产版本 (跨平台)
bun run tauri build
```

## 📖 使用指南

### 初次启动
1. 启动 Magic Claude
2. 如果尚未安装 Claude CLI，应用会提供下载指引
3. 应用已预配置 Magic666.top 服务地址
4. 在设置中添加您的 API 密钥即可开始使用

### Magic666 服务配置
1. 打开**设置** → **代理商**标签
2. 点击**添加代理商**配置您的 Magic666 服务
3. 填写服务信息：
   - **名称**: 服务的显示名称（如 "Magic666 主服务"）
   - **描述**: 可选的描述信息
   - **API 地址**: 已锁定为 https://magic666.top
   - **认证Token** 或 **API Key**: 输入您的 Magic666.top API 密钥
   - **模型**: 可选的默认模型

### 项目管理
- **创建项目**: 在主界面点击"新建项目"
- **会话管理**: 每个项目支持多个会话，保持上下文连续性
- **检查点系统**: 关键节点自动保存，支持回滚操作

## 🛠️ 技术架构

### 前端技术栈
- **React 18** - 现代化的用户界面框架
- **TypeScript** - 类型安全的开发体验
- **Tailwind CSS 4** - 实用优先的 CSS 框架
- **Framer Motion** - 流畅的动画效果
- **i18next** - 国际化支持

### 后端技术栈
- **Tauri 2** - 现代化的跨平台桌面应用框架
- **Rust** - 高性能的系统编程语言
- **SQLite** - 嵌入式数据库
- **系统 API** - 原生系统集成（Windows/macOS/Linux）

### 核心架构
```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   React 前端    │◄──►│   Tauri 桥接    │◄──►│   Rust 后端     │
│                 │    │                 │    │                 │
│ • UI 组件       │    │ • IPC 通信      │    │ • Claude CLI    │
│ • 状态管理      │    │ • 安全调用      │    │ • 进程管理      │
│ • 路由系统      │    │ • 类型安全      │    │ • Windows API   │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

## 🤝 贡献指南

我们欢迎所有形式的贡献！

### 开发环境准备
1. Fork 本仓库到您的 GitHub 账户
2. 克隆您的 Fork 到本地
3. 安装依赖：`bun install`
4. 启动开发服务器：`bun run tauri dev`

### 提交规范
- 使用清晰的提交信息
- 遵循现有的代码风格
- 添加适当的测试覆盖
- 更新相关文档

### 报告问题
- 使用 [Issue 模板](https://github.com/anyme123/magic-claude/issues/new) 报告 Bug
- 提供详细的复现步骤和环境信息
- 附加相关的日志文件和截图
- 联系 Magic666.top 技术支持获取 API 相关帮助

## 📝 更新日志

### v1.0.0 (2025-07-29)
- 🎉 Magic Claude 正式发布
- ✨ 完整的 Claude 项目管理功能
- 🔧 集成 Magic666.top 专业 API 服务
- 🌍 中文优先的多语言支持
- 🎨 现代化的用户界面设计
- 🖥️ 跨平台支持（Windows/macOS/Linux）
- 🔒 API 地址安全锁定机制

## 📄 许可证

本项目基于 [MIT License](LICENSE) 开源协议发布。

## 🙏 致谢

- **Magic666.top** - 提供稳定可靠的 Claude API 服务和技术支持
- **原项目致谢** - 感谢 [@getAsterisk/claudia](https://github.com/getAsterisk/claudia) 提供的基础架构和灵感

- [Claude](https://claude.ai/) - 强大的 AI 助手
- [Tauri](https://tauri.app/) - 现代化的桌面应用框架  
- [React](https://react.dev/) - 用户界面构建库
- [Rust](https://rust-lang.org/) - 系统编程语言

## 📞 联系方式

- **GitHub**: [GitHub Issues](https://github.com/anyme123/magic-claude/issues)
- **Discussions**: [GitHub Discussions](https://github.com/anyme123/magic-claude/discussions)
- **Magic666.top**: [官方网站](https://magic666.top) - API 服务和技术支持
- **技术支持**: 访问 Magic666.top 获取专业的 API 服务支持

---

<div align="center">
  <p>如果这个项目对您有帮助，请考虑给我们一个 ⭐</p>
  <p>Made with ❤️ by Magic666.top team</p>
  <p><a href="https://magic666.top">🔗 访问 Magic666.top 获取 API 服务</a></p>
</div>
