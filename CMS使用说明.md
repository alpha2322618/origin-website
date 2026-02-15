# Origin 网站 CMS 使用说明

## 🌐 网站地址
**https://6h7xuohmdlcm4.ok.kimi.link**

## 📝 后台管理地址
**https://6h7xuohmdlcm4.ok.kimi.link/admin/simple.html**

---

## 📋 功能介绍

我已经为你的网站添加了 **内容管理系统 (CMS)**，你可以通过后台管理界面轻松修改网站内容，无需编写代码！

### 可管理的内容

1. **联系方式** - 微信、QQ、电话、邮箱
2. **首页横幅** - 中文标题、英文标题、副标题
3. **特色卡片** - 4个特色卡片的标题和描述
4. **关于起源** - 标题、副标题、两段内容
5. **CTA区域** - 主标题、副标题、按钮文字
6. **新闻资讯** - 添加/编辑新闻文章（需手动修改文件）

---

## 🚀 如何使用

### 方法一：使用在线管理界面（推荐）

1. 访问 **https://6h7xuohmdlcm4.ok.kimi.link/admin/simple.html**
2. 点击顶部的标签切换不同的设置页面
3. 修改内容后点击「保存」按钮
4. 下载生成的 JSON 文件
5. 将文件替换到 `content/` 文件夹中
6. 重新构建并部署网站

### 方法二：直接编辑 JSON 文件

如果你熟悉文件操作，可以直接编辑 `content/` 文件夹中的 JSON 文件：

```
content/
├── contact.json      # 联系方式
├── hero.json         # 首页横幅
├── features.json     # 特色卡片
├── about.json        # 关于起源
├── cta.json          # CTA区域
├── news/             # 新闻文章
│   ├── 2026-02-15-origin-trilogy.md
│   ├── 2026-02-15-lgns-price.md
│   └── 2026-02-14-wealth-opportunity.md
└── ecosystem/        # 生态系统
    ├── version-1.md
    ├── version-2.md
    └── version-3.md
```

---

## 📁 文件格式说明

### contact.json - 联系方式
```json
{
  "wechat": "107241795",
  "qq": "107241795",
  "phone": "17675761558",
  "email": "contact@origin.pub"
}
```

### hero.json - 首页横幅
```json
{
  "chineseTitle": "起 源",
  "englishTitle": "ORIGIN",
  "subtitle": "革新金融自由  捍卫人类财富隐私"
}
```

### features.json - 特色卡片
```json
{
  "items": [
    {
      "title": "本金安全",
      "description": "137套智能合约...",
      "icon": "Shield"
    }
  ]
}
```

### about.json - 关于起源
```json
{
  "title": "关于起源（Origin）",
  "subtitle": "欢迎来到起源银行（Origin）",
  "paragraph1": "第一段内容...",
  "paragraph2": "第二段内容..."
}
```

### cta.json - CTA区域
```json
{
  "title": "原创经济模型...",
  "subtitle": "暗网出品  必属精品",
  "buttonText": "打开财富大门"
}
```

---

## 🔄 更新网站流程

### 方式一：使用 Vercel/Netlify（推荐，自动部署）

1. 将代码上传到 GitHub
2. 在 Vercel/Netlify 导入项目
3. 修改 `content/` 文件夹中的内容
4. 提交到 GitHub
5. 自动重新部署

### 方式二：手动部署

1. 修改 `content/` 文件夹中的 JSON 文件
2. 运行 `npm run build` 重新构建
3. 将 `dist/` 文件夹部署到服务器

---

## 💡 常见问题

### Q: 修改后为什么没有生效？
A: 需要重新构建并部署网站才能看到更新。

### Q: 如何添加新闻？
A: 在 `content/news/` 文件夹中创建新的 `.md` 文件，参考现有文件的格式。

### Q: 如何修改图片？
A: 将新图片放到 `public/images/` 文件夹，然后在 JSON 中引用新路径。

### Q: 可以添加更多内容吗？
A: 可以！联系我帮你添加更多可管理的内容类型。

---

## 📞 需要帮助？

如果你在使用过程中遇到任何问题，随时联系我！
