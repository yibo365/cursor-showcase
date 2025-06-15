# AI Coding Agent 完整分享

> 基于 Slidev 构建的 AI 编程助手演示文稿

## 🚀 项目简介

这是一个完整的 AI Coding Agent 分享演示，涵盖了从 Chat 到 Agent 的 AI 编程助手进化史，以及 Cursor 的深度使用指南和最佳实践。

## 📁 项目结构

```
cursor-demo/
├── slides.md           # 主要演示文稿内容
├── public/
│   └── images/         # 演示图片资源
├── vercel.json         # Vercel 部署配置
├── package.json        # 项目依赖
└── README.md           # 项目说明
```

## 🛠️ 本地开发

### 安装依赖
```bash
npm install
```

### 启动开发服务器
```bash
npm run dev
```

### 构建生产版本
```bash
npm run build
```

## 🌐 部署到 Vercel

### 方法一：通过 GitHub 导入（推荐）

1. 访问 [Vercel](https://vercel.com)
2. 点击 "New Project"
3. 导入 GitHub 仓库：`https://github.com/yibo365/cursor-showcase`
4. 选择 `cursor-demo` 目录作为根目录
5. Vercel 会自动检测到 `vercel.json` 配置并部署

### 方法二：通过 Vercel CLI

```bash
# 安装 Vercel CLI
npm i -g vercel

# 登录 Vercel
vercel login

# 部署项目
vercel --prod
```

## 📖 演示内容

- **AI 编程进化史**：从 Chat → Copilot → Agent → Engineer 的演进
- **Cursor 核心功能**：Tab 补全、Cmd K 编辑、Chat/Agent 模式
- **上下文符号系统**：@ 符号的强大功能
- **高级功能**：MCP、Beta 功能、模型选择策略
- **最佳实践**：个人和团队的使用经验分享
- **产品对比**：市场主要 AI 编程工具对比分析

## 🎯 特色功能

- ✅ 完整的 AI 编程助手知识体系
- ✅ 实用的 Cursor 使用技巧和最佳实践
- ✅ 丰富的产品对比和选择建议
- ✅ 美观的 Slidev 演示界面
- ✅ 支持一键部署到 Vercel

## 📝 使用说明

1. **演示导航**：使用方向键或点击进行页面切换
2. **全屏模式**：按 `F` 键进入全屏演示
3. **演示者模式**：按 `P` 键进入演示者模式
4. **打印导出**：访问 `/print` 路径可打印或导出 PDF

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个演示！

## 📄 许可证

MIT License

---

**Made with ❤️ using Slidev**
