# Origin 网站 - Vercel 自动部署版

Origin 起源银行官方网站，基于 React + TypeScript + Tailwind CSS 构建，支持 CMS 内容管理。

## 🌐 在线预览

部署后你的网站将可以通过 Vercel 提供的域名访问。

## 🚀 快速开始

### 1. 部署到 Vercel（推荐）

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)

点击上方按钮，选择你的 GitHub 仓库，一键部署！

### 2. 本地开发

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build
```

## 📁 项目结构

```
├── content/              # CMS 内容文件夹
│   ├── contact.json      # 联系方式
│   ├── hero.json         # 首页横幅
│   ├── features.json     # 特色卡片
│   ├── about.json        # 关于起源
│   ├── cta.json          # CTA区域
│   ├── news/             # 新闻文章
│   └── ecosystem/        # 生态系统
├── public/
│   ├── admin/            # 后台管理界面
│   └── images/           # 图片资源
├── src/
│   ├── sections/         # 页面组件
│   └── hooks/            # 数据加载 hooks
├── package.json
├── tailwind.config.js
├── tsconfig.json
└── vite.config.ts
```

## 📝 内容管理

### 方式一：使用管理界面

1. 访问 `https://你的域名/admin/simple.html`
2. 修改内容并下载 JSON 文件
3. 将文件放到 `content/` 文件夹
4. 提交到 GitHub，自动部署

### 方式二：直接编辑文件

直接修改 `content/` 文件夹中的 JSON 文件，然后提交到 GitHub。

## 🔄 自动部署流程

```
修改 content/xxx.json → 提交到 GitHub → Vercel 自动构建 → 网站更新
```

## 📞 联系方式

- 微信：107241795
- QQ：107241795
- 电话：17675761558

## 📄 许可证

MIT License
