# heiqi-cli

一个简单的脚手架工具，用于快速创建和管理项目。

## 功能特性

- 🚀 快速创建项目
- 📦 自动安装依赖
- 🎯 自动启动项目
- 🔄 支持项目更新

## 安装

```bash
npm install heiqi-cli -g
```

## 使用方法

### 创建项目

```bash
heiqi create <project-name>
```

### 更新脚手架

```bash
heiqi update
```

## 项目结构

```
heiqi-cli/
├── src/
│   ├── command/        # 命令实现
│   ├── utils/          # 工具函数
│   └── index.ts        # 入口文件
├── package.json
└── README.md
```

## 开发

```bash
# 安装依赖
pnpm install

# 开发模式
pnpm run dev

# 构建
pnpm run build
```

## 依赖说明

### 核心依赖

- `@inquirer/prompts`: 命令行交互工具，提供文本输入、选择列表等交互组件
- `chalk`: 命令行输出美化工具，支持彩色文本输出
- `commander`: 命令行工具开发框架，用于创建命令和子命令
- `log-symbols`: 命令行日志符号，提供统一的日志标识
- `ora`: 命令行加载动画，用于显示长时间运行的操作进度
- `progress-estimator`: 进度估算工具，显示操作进度和预估时间
- `simple-git`: Git 操作封装，提供简单的 Git 命令接口

### 开发依赖

- `@rollup/plugin-commonjs`: Rollup 插件，支持 CommonJS 模块转换
- `@rollup/plugin-json`: Rollup 插件，支持 JSON 文件导入
- `@rollup/plugin-node-resolve`: Rollup 插件，用于解析 Node.js 模块
- `@rollup/plugin-terser`: Rollup 插件，用于代码压缩和混淆
- `rollup-plugin-esbuild`: Rollup 插件，使用 ESBuild 进行代码转换
- `rollup-plugin-node-externals`: Rollup 插件，自动识别外部依赖
- `rollup-plugin-typescript2`: Rollup 插件，支持 TypeScript 编译

### TypeScript 相关

- `@types/fs-extra`: fs-extra 的类型定义
- `@types/lodash`: lodash 的类型定义
- `@types/node`: Node.js 的类型定义
- `tslib`: TypeScript 运行时库
- `typescript`: TypeScript 编译器

### 工具库

- `axios`: HTTP 客户端，用于发起网络请求
- `fs-extra`: 文件系统操作扩展库
- `lodash`: 实用工具函数库

## License

MIT 