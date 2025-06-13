# Cursor AI 编程助手演示

这是一个使用 [Slidev](https://sli.dev) 创建的演示文稿，用于展示 Cursor AI 编程助手的强大功能。

## 🚀 快速开始

### 安装依赖
```bash
pnpm install
```

### 启动开发服务器
```bash
pnpm dev
```

浏览器会自动打开 `http://localhost:3030`，你就可以看到演示文稿了。

### 导出 PDF
```bash
pnpm export
```

## 📋 演示内容

这个演示文稿包含以下主要内容：

1. **Cursor 简介** - 什么是 Cursor，为什么选择它
2. **核心功能演示**：
   - Tab 智能补全
   - Cmd+K 快速编辑
   - Cmd+L 对话编程
3. **实战演示**：
   - 从零创建 React 组件
   - 调试和修复错误
   - 代码重构和优化
   - AI 辅助学习新技术
4. **最佳实践** - 如何最大化 Cursor 的效能
5. **团队协作** - 在团队中推广 Cursor
6. **未来展望** - AI 编程的发展趋势

## 🎯 演示技巧

### 键盘快捷键
- `空格键` 或 `→` - 下一页/下一个动画
- `←` - 上一页/上一个动画
- `f` - 全屏模式
- `o` - 演示者模式
- `d` - 深色模式切换

### 演示者模式
按 `o` 键进入演示者模式，可以看到：
- 当前幻灯片和下一张幻灯片的预览
- 演示者备注
- 计时器
- 幻灯片导航

## 📁 项目结构

```
cursor-demo/
├── slides.md                 # 主要的幻灯片内容
├── cursor-architecture.mmd   # Cursor 架构图
├── package.json              # 项目配置
├── components/               # 自定义组件
├── pages/                    # 额外的页面
└── snippets/                 # 代码片段
```

## 🛠 自定义

### 修改内容
编辑 `slides.md` 文件来修改幻灯片内容。Slidev 支持：
- Markdown 语法
- Vue 组件
- 代码高亮
- Mermaid 图表
- LaTeX 数学公式
- 动画效果

### 更换主题
在 `slides.md` 的 frontmatter 中修改 `theme` 字段：
```yaml
---
theme: seriph  # 或者 default, apple, etc.
---
```

### 添加自定义样式
可以在幻灯片中使用 `<style>` 标签添加自定义 CSS。

## 📚 相关资源

- [Slidev 官方文档](https://sli.dev)
- [Cursor 官网](https://cursor.sh)
- [Cursor 官方文档](https://docs.cursor.sh)
- [Mermaid 图表语法](https://mermaid.js.org)

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个演示项目！

## �� 许可证

MIT License
