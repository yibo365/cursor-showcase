---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://images.unsplash.com/photo-1555066931-4365d14bab8c?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80
# some information about your slides (markdown enabled)
title: Cursor AI 编程助手演示
info: |
  ## Cursor AI 编程助手完整演示
  
  展示如何使用 Cursor 提升开发效率
  
  演示者：Eric
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# open graph
# seoMeta:
#  ogImage: https://cover.sli.dev
---

# Cursor AI 编程助手

## 让 AI 成为你的编程伙伴

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover:bg="white hover:bg-opacity-10">
    开始演示 <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="在编辑器中打开" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://cursor.sh" target="_blank" alt="Cursor 官网" title="Cursor 官网"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:code />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---

# 什么是 Cursor？

Cursor 是一款基于 AI 的代码编辑器，专为提升开发效率而设计

<v-clicks>

- 🤖 **AI 原生** - 内置 GPT-4 等先进 AI 模型
- ⚡ **智能补全** - 上下文感知的代码建议
- 💬 **对话编程** - 与 AI 直接对话解决问题
- 🔧 **代码重构** - AI 辅助的代码优化和重构
- 📝 **文档生成** - 自动生成代码注释和文档
- 🐛 **错误修复** - 智能识别并修复代码问题
- 🎯 **多语言支持** - 支持主流编程语言

</v-clicks>

<br>

<v-click>

## 为什么选择 Cursor？

传统编辑器 + AI 插件 ❌  
**AI 原生编辑器** ✅

</v-click>

---
layout: two-cols
layoutClass: gap-16
---

# 演示大纲

今天我们将展示 Cursor 的核心功能：

<Toc minDepth="1" maxDepth="2" />

::right::

## 演示环境

- **编辑器**: Cursor
- **AI 模型**: GPT-4
- **项目类型**: 
  - React/TypeScript 应用
  - Node.js 后端
  - Python 脚本
- **演示重点**: 
  - 实际开发场景
  - 效率对比
  - 最佳实践

---

# 核心功能 1：智能代码补全

## Tab 补全 - 预测你的下一步

<div class="grid grid-cols-2 gap-8 mt-8">

<div>

### 传统补全
```typescript
// 只能补全已知的方法和属性
const user = {
  name: 'John',
  age: 30
}
user.// 只显示 name, age
```

</div>

<div>

### Cursor AI 补全
```typescript {all|3-8|all}
// 理解上下文，预测整个代码块
const user = {
  name: 'John',
  age: 30
}
// AI 预测你想要的功能
const greeting = `Hello, ${user.name}! You are ${user.age} years old.`
const isAdult = user.age >= 18
```

</div>

</div>

<v-click>

## 🎯 演示重点
- **上下文理解**：AI 理解代码意图
- **多行预测**：不只是单个方法，而是整个逻辑块
- **智能建议**：基于最佳实践的代码建议

</v-click>

---

# 核心功能 2：Cmd+K 快速编辑

## 自然语言描述，AI 直接实现

<div class="mt-8">

### 使用场景示例

<v-clicks>

1. **"添加错误处理"** → AI 自动添加 try-catch 块
2. **"优化这个函数的性能"** → AI 重构代码逻辑
3. **"添加 TypeScript 类型"** → AI 推断并添加类型定义
4. **"重构为 React Hook"** → AI 将组件逻辑提取为自定义 Hook
5. **"添加单元测试"** → AI 生成对应的测试用例

</v-clicks>

</div>

<v-click>

<div class="mt-8 p-4 bg-blue-50 rounded-lg">

### 💡 演示技巧
- 选中代码块后使用 `Cmd+K`
- 用自然语言描述需求
- AI 会在原地修改代码
- 可以撤销和重新生成

</div>

</v-click>

---

# 核心功能 3：Cmd+L 对话编程

## 与 AI 结对编程

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### 对话场景
- 🤔 **解释代码**："这段代码是做什么的？"
- 🐛 **调试问题**："为什么这个函数返回 undefined？"
- 🔧 **架构建议**："如何重构这个组件？"
- 📚 **学习新技术**："如何使用 React Query？"
- 🎯 **代码审查**："这段代码有什么问题？"

</div>

<div>

### 对话优势
- **上下文感知**：AI 能看到整个项目
- **实时交互**：即问即答
- **代码生成**：直接插入到编辑器
- **多轮对话**：持续深入讨论
- **学习助手**：解释概念和最佳实践

</div>

</div>

<v-click>

<div class="mt-6 p-4 bg-green-50 rounded-lg">

### 🚀 实战演示
接下来我们将通过实际项目演示这些功能的强大之处！

</div>

</v-click>

---
layout: center
class: text-center
---

# 实战演示

## 让我们看看 Cursor 的真正威力

<div class="mt-8">
  <div class="text-6xl mb-4">🚀</div>
  <div class="text-xl opacity-80">准备好被震撼了吗？</div>
</div>

---

# 演示 1：从零创建 React 组件

## 场景：创建一个待办事项组件

<div class="mt-6">

### 演示步骤

<v-clicks>

1. **创建新文件** `TodoList.tsx`
2. **使用 Tab 补全** 快速搭建组件结构
3. **Cmd+K 添加功能**：
   - "添加新增待办功能"
   - "添加删除功能"
   - "添加完成状态切换"
4. **Cmd+L 优化代码**：
   - "使用 TypeScript 严格类型"
   - "添加样式美化"
   - "优化性能"

</v-clicks>

</div>

<v-click>

<div class="mt-6 p-4 bg-yellow-50 rounded-lg">

### ⏱️ 时间对比
- **传统开发**：30-45 分钟
- **使用 Cursor**：5-10 分钟

</div>

</v-click>

---

# 演示 2：调试和修复错误

## 场景：修复一个复杂的异步数据获取问题

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### 问题代码
```typescript
// 有 bug 的代码
const fetchUserData = async () => {
  const response = fetch('/api/users')
  const data = response.json()
  setUsers(data.users)
}
```

</div>

<div>

### Cursor 修复过程
<v-clicks>

1. **AI 识别问题**：缺少 await 关键字
2. **建议修复**：添加错误处理
3. **优化建议**：使用更好的错误处理模式
4. **类型安全**：添加 TypeScript 类型

</v-clicks>

</div>

</div>

<v-click>

### 修复后的代码
```typescript
const fetchUserData = async (): Promise<void> => {
  try {
    const response = await fetch('/api/users')
    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`)
    }
    const data: { users: User[] } = await response.json()
    setUsers(data.users)
  } catch (error) {
    console.error('Failed to fetch users:', error)
    setError('Failed to load users')
  }
}
```

</v-click>

---

# 演示 3：代码重构和优化

## 场景：将类组件重构为函数组件 + Hooks

<div class="mt-6">

### 重构挑战
- 复杂的状态管理
- 生命周期方法转换
- 性能优化
- 类型定义更新

</div>

<v-click>

<div class="mt-6">

### Cursor 的解决方案
1. **选中整个类组件**
2. **Cmd+K**: "重构为函数组件，使用 React Hooks"
3. **AI 自动处理**：
   - `useState` 替换 `this.state`
   - `useEffect` 替换生命周期方法
   - `useCallback` 优化性能
   - 更新 TypeScript 类型

</div>

</v-click>

<v-click>

<div class="mt-6 p-4 bg-purple-50 rounded-lg">

### 🎯 结果
- **代码行数减少** 40%
- **性能提升** 明显
- **类型安全** 增强
- **可维护性** 大幅提升

</div>

</v-click>

---

# 演示 4：AI 辅助学习新技术

## 场景：学习并实现 React Query

<div class="mt-6">

### 学习过程

<v-clicks>

1. **Cmd+L 询问**："如何在 React 中使用 React Query？"
2. **AI 解释概念**：缓存、同步、错误处理
3. **生成示例代码**：完整的实现示例
4. **最佳实践建议**：错误边界、加载状态等
5. **实际应用**：在项目中集成

</v-clicks>

</div>

<v-click>

<div class="mt-6 grid grid-cols-2 gap-8">

<div>

### 传统学习方式
- 📖 阅读文档
- 🔍 搜索示例
- 💻 手动编写代码
- 🐛 调试错误
- ⏰ 耗时 2-3 小时

</div>

<div>

### Cursor 辅助学习
- 💬 直接对话询问
- 🤖 AI 解释概念
- ⚡ 即时生成代码
- 🔧 自动修复问题
- ⏰ 耗时 20-30 分钟

</div>

</div>

</v-click>

---

# 高级技巧和最佳实践

## 让 Cursor 发挥最大效能

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### 🎯 使用技巧

<v-clicks>

- **明确的指令**：具体描述需求
- **上下文提供**：选中相关代码
- **迭代优化**：多轮对话完善
- **代码审查**：让 AI 检查代码质量
- **学习模式**：询问"为什么"和"如何"

</v-clicks>

</div>

<div>

### ⚠️ 注意事项

<v-clicks>

- **验证输出**：AI 生成的代码需要检查
- **安全考虑**：敏感信息不要暴露
- **版本控制**：及时提交代码变更
- **测试覆盖**：确保功能正确性
- **性能监控**：关注代码性能影响

</v-clicks>

</div>

</div>

<v-click>

<div class="mt-8 p-4 bg-blue-50 rounded-lg">

### 💡 专业建议
Cursor 是工具，不是替代品。最好的效果来自于**人机协作**，而不是完全依赖 AI。

</div>

</v-click>

---

# 效率提升数据

## 真实的开发效率对比

<div class="mt-8">

<div class="grid grid-cols-3 gap-8">

<div class="text-center">
<div class="text-4xl font-bold text-green-600">3-5x</div>
<div class="text-sm opacity-75">代码编写速度</div>
</div>

<div class="text-center">
<div class="text-4xl font-bold text-blue-600">70%</div>
<div class="text-sm opacity-75">调试时间减少</div>
</div>

<div class="text-center">
<div class="text-4xl font-bold text-purple-600">80%</div>
<div class="text-sm opacity-75">重复工作减少</div>
</div>

</div>

</div>

<v-click>

<div class="mt-8">

### 📊 具体场景提升

| 开发任务 | 传统方式 | 使用 Cursor | 提升比例 |
|---------|---------|------------|---------|
| 创建 CRUD 接口 | 2 小时 | 30 分钟 | **4x** |
| 编写单元测试 | 1.5 小时 | 20 分钟 | **4.5x** |
| 代码重构 | 3 小时 | 45 分钟 | **4x** |
| 学习新框架 | 1 天 | 2 小时 | **4x** |
| 调试复杂问题 | 2 小时 | 30 分钟 | **4x** |

</div>

</v-click>

---

# 团队协作和最佳实践

## 在团队中推广 Cursor

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### 🏢 团队采用策略

<v-clicks>

1. **试点项目**：选择小项目开始
2. **培训分享**：组织内部培训
3. **最佳实践**：建立使用规范
4. **代码审查**：确保代码质量
5. **效果评估**：量化提升效果

</v-clicks>

</div>

<div>

### 📋 团队规范建议

<v-clicks>

- **代码风格**：统一 AI 生成代码的风格
- **安全规范**：敏感信息处理规则
- **质量标准**：AI 代码的审查标准
- **文档要求**：AI 生成代码的文档
- **测试覆盖**：确保测试完整性

</v-clicks>

</div>

</div>

<v-click>

<div class="mt-8 p-4 bg-orange-50 rounded-lg">

### 🎯 成功关键
团队成功采用 Cursor 的关键在于**渐进式引入**和**持续学习**，而不是一次性替换所有工具。

</div>

</v-click>

---

# 未来展望

## AI 编程的发展趋势

<div class="mt-8">

<v-clicks>

- 🧠 **更智能的 AI**：GPT-5、Claude 等新模型
- 🔗 **更好的集成**：与更多开发工具深度集成
- 🎯 **专业化模型**：针对特定语言和框架优化
- 🤝 **团队协作**：AI 辅助的团队开发
- 🔒 **企业级功能**：更好的安全性和隐私保护
- 📱 **移动开发**：移动端 AI 编程工具
- 🌐 **云端协作**：基于云的 AI 开发环境

</v-clicks>

</div>

<v-click>

<div class="mt-8 p-4 bg-gradient-to-r from-blue-50 to-purple-50 rounded-lg">

### 🚀 我们正处在编程革命的起点

AI 不会取代程序员，但**会使用 AI 的程序员会取代不会使用 AI 的程序员**。

</div>

</v-click>

---
layout: center
class: text-center
---

# Q&A 环节

## 有什么问题想要了解的吗？

<div class="mt-8 text-6xl">🤔</div>

<div class="mt-8 grid grid-cols-3 gap-8 text-sm">

<div>
**功能相关**
- 具体使用技巧
- 高级功能探索
- 性能优化建议
</div>

<div>
**实践相关**
- 项目集成方案
- 团队推广经验
- 最佳实践分享
</div>

<div>
**技术相关**
- 与其他工具对比
- 特定场景应用
- 未来发展讨论
</div>

</div>

---
layout: center
class: text-center
---

# 感谢观看！

## 开始你的 AI 编程之旅

<div class="mt-8">
  <div class="text-4xl mb-4">🎉</div>
  <div class="text-xl opacity-80 mb-8">希望这次演示对你有帮助</div>
</div>

<div class="flex justify-center gap-8 text-sm">
  <div>
    <div class="font-bold mb-2">🔗 相关链接</div>
    <div><a href="https://cursor.sh" target="_blank">Cursor 官网</a></div>
    <div><a href="https://docs.cursor.sh" target="_blank">官方文档</a></div>
  </div>
  <div>
    <div class="font-bold mb-2">📧 联系方式</div>
    <div>邮箱：your-email@example.com</div>
    <div>GitHub：@your-github</div>
  </div>
</div>

<div class="mt-8 text-xs opacity-60">
  演示文稿使用 <a href="https://sli.dev" target="_blank">Slidev</a> 制作
</div>
