# Dashboard Project

这是一个学习 Next.js App Router 课程的仪表板项目，包含了基本的仪表盘功能和用户界面。

## 项目概述

该项目是一个现代化的仪表板应用，使用 Next.js App Router 构建，展示了如何使用最新的 Next.js 特性来构建生产级别的应用程序。

## 功能特性

- 📊 仪表板统计数据展示
- 👥 客户管理系统
- 💸 发票管理系统
- 🔍 搜索功能
- 📱 响应式设计
- 🔒 用户认证系统

## 技术栈

- **框架**: Next.js 14 (App Router)
- **语言**: TypeScript
- **样式**: Tailwind CSS
- **认证**: NextAuth.js
- **数据库**: PostgreSQL
- **ORM**: Postgres.js (Raw SQL)
- **验证**: Zod
- **工具**: 
  - clsx (类名操作)
  - use-debounce (防抖功能)
  - bcrypt (密码哈希)

## 快速开始

### 安装依赖

```bash
pnpm install
```

### 配置环境变量

创建 `.env` 文件并填写以下内容：

```env
DATABASE_URL=your_postgresql_url
AUTH_SECRET=your_auth_secret
```

可以参考 `.env.example` 文件获取更多配置选项。

### 初始化数据库

```bash
pnpm run seed
```

### 运行开发服务器

```bash
pnpm run dev
```

应用将在 `http://localhost:3000` 启动

### 构建生产版本

```bash
pnpm run build
```

### 启动生产服务器

```bash
pnpm run start
```

## 项目结构

```
dashboard/
├── app/
│   ├── layout.tsx              # 根布局组件
│   ├── page.tsx                # 首页
│   ├── lib/                    # 共享库和工具函数
│   │   ├── data.ts             # 数据访问层
│   │   ├── definitions.ts      # TypeScript 类型定义
│   │   ├── placeholder-data.ts # 占位符数据
│   │   └── utils.ts            # 工具函数
│   ├── query/                  # API 路由 - 查询
│   ├── seed/                   # API 路由 - 数据库种子
│   └── ui/                     # UI 组件
│       ├── dashboard/          # 仪表盘相关组件
│       ├── invoices/           # 发票相关组件
│       ├── customers/          # 客户相关组件
│       └── global.css          # 全局样式
├── public/                     # 静态资源
├── next.config.ts              # Next.js 配置
├── tailwind.config.ts          # Tailwind 配置
├── postcss.config.js           # PostCSS 配置
├── tsconfig.json               # TypeScript 配置
└── package.json                # 项目依赖
```

## 学习资源

- [Next.js App Router 官方文档](https://nextjs.org/docs/app)
- [Next.js 学习课程](https://nextjs.org/learn)
- [Tailwind CSS 官方文档](https://tailwindcss.com/docs)

## License

MIT
