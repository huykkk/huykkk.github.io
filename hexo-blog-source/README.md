# Huyk Blog - PM小白的快落小屋

你的 Hexo 博客源码已从 GitHub Pages 编译产物中成功重建。

## 在新电脑上使用

### 1. 安装依赖

```bash
cd hexo-blog-source
npm install
```

### 2. 本地预览

```bash
npx hexo server
```

打开 http://localhost:4000 即可预览。

### 3. 写新文章

```bash
npx hexo new "我的新文章标题"
```

文章会生成在 `source/_posts/` 目录下，用 Markdown 编写。

### 4. 生成静态文件

```bash
npx hexo generate
```

### 5. 部署到 GitHub Pages

```bash
npx hexo deploy
```

> 部署需要配置 Git 凭据，建议使用 GitHub Token 或 SSH Key。

## 项目结构

```
hexo-blog-source/
├── _config.yml          # Hexo 配置文件
├── source/
│   ├── _posts/          # 博客文章（13 篇已恢复）
│   ├── about/           # 关于页面
│   ├── gallery/         # 文章封面图
│   └── img/             # 网站图片资源
├── themes/              # 主题（默认 landscape）
└── scaffolds/           # 文章模板
```

## 已恢复的文章（13 篇）

| 日期 | 标题 | 分类 |
|------|------|------|
| 2021-09-01 | git操作指南 | 学习/前端 |
| 2021-09-01 | toB产品需求调研 | 学习/产品 |
| 2021-09-01 | 产品思考 | 学习/产品 |
| 2021-09-01 | 梁宁产品思维三十讲 | 学习/产品 |
| 2021-09-03 | typora+picgo+github = 编辑器+图床 | 学习/知识 |
| 2021-09-06 | 大变局下的中国管理 | 学习/知识 |
| 2021-09-22 | 个人总结B端产品工作流 | 学习/产品 |
| 2021-10-15 | 产品经理PRD文档规范 | 学习/产品 |
| 2021-10-20 | 工作流&审批流的思考 | 学习/产品 |
| 2021-10-21 | 后台管理系统界面框架 | 学习/前端 |
| 2021-10-27 | ERP系统业务总结 | 学习/产品 |
| 2021-11-12 | 原型设计软件笔记-Figma | 学习/产品 |
| 2021-11-17 | 读《金融的谜题》笔记 | 学习/知识 |

## 配置说明

`_config.yml` 已配置好：
- 网站标题、作者、语言
- URL 指向 `https://huykkk.github.io`
- 部署目标：`huykkk/huykkk.github.io` 仓库的 `gh-pages` 分支

如需更换主题，可以安装其他 Hexo 主题（如 NexT、Butterfly 等）。
