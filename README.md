

# Spring-AI-Test-FrontEnd

基于 **Vue 3** + **TypeScript** + **Vite** 构建的现代前端应用，提供高效开发体验。

---

## 🚀 项目概述

本项目为构建 Web 应用提供标准化开发环境，整合 Vue 3 的组合式 API、TypeScript 的类型安全特性以及 Vite 的极速构建能力，支持快速开发与生产级优化。

---

## 🧰 技术栈

| 技术             | 角色    | 核心优势                          |
| -------------- | ----- | ----------------------------- |
| **Vue 3**      | 前端框架  | 组件化架构、响应式系统、组合式 API           |
| **TypeScript** | 类型化语言 | 静态类型检查、代码智能提示、更易维护            |
| **Vite**       | 构建工具  | 即时启动开发服务器、热模块更新（HMR）、生产环境优化打包 |

---

## 🛠️ 开发环境搭建

1. **克隆项目**
   ```bash
   git clone https://github.com/LuciusWan/Spring-AI-Agent-FrontEnd.git

2. **安装依赖**
   
   ```bash
   npm install
   ```

3. **VSCode 配置**
   
   - 安装 **Volar** 扩展（Vue 3 专用支持）
   - 禁用 **Vetur** 避免冲突
   - 启用 TypeScript 对 `.vue` 文件的类型解析

4. **启动开发服务器**
   
   ```bash
   npm run dev
   ```
   
   - 特性：
     - 热模块替换（HMR）实时更新
     - 浏览器预览（默认地址 `http://localhost:5173`）
     - 通过 Volar 实现 IDE 内类型检查

---

## 🔧 开发与构建流程

### 开发模式流程

```
.vue 文件
↓
Vite 开发服务器
├─ TypeScript 语言服务（类型检查）
└─ 浏览器实时预览 + HMR
```

### 生产构建流程

```
.vue 文件
↓
vue-tsc 类型检查
↓
Vite 构建
└─ 资源压缩优化
└─ 输出 HTML/CSS/JS 生产包
```

---

## 📁 项目结构

```
project-root/
├── public/              # 静态资源（无需编译）
├── src/                 # 源代码目录
│   ├── assets/          # 可编译资源（图片/样式等）
│   ├── components/      # Vue 组件
│   └── main.ts          # 入口文件
├── tsconfig.json        # TypeScript 配置
├── vite.config.ts       # Vite 构建配置
└── package.json         # 项目依赖与脚本
```

---

## 📦 主要脚本说明

| 命令                | 功能             |
| ----------------- | -------------- |
| `npm run dev`     | 启动开发服务器（带 HMR） |
| `npm run build`   | 类型检查 + 生产构建    |
| `npm run preview` | 预览生产构建结果       |

---

## 🤝 贡献指南

1. Fork 项目并创建开发分支
2. 提交 PR 前确保通过类型检查（`npm run build`）
3. 遵循 Vue 3 + TypeScript 最佳实践

---

## 📌 常见问题

- **Q：如何修复 `.vue` 文件类型错误？**  
  A：确保已安装 Volar 扩展，并在 VSCode 设置中禁用 Vetur。

- **Q：生产构建后资源路径异常？**  
  A：检查 `vite.config.ts` 中的 `base` 配置项。

- **Q：如何自定义主题样式？**  
  A：在 `src/assets/styles` 目录下修改 SCSS 变量文件。

---

本项目持续优化中，欢迎提出 issue 或提交 PR 协助完善！
