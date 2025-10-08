# eatingwang012.github.io

## 🎯 项目简介

这是一个基于React + TypeScript + Tailwind CSS构建的个人作品集网站，展示了我的AI项目、设计作品和工作经验。

## ✨ 特性

- 🚀 **现代化设计** - 使用Tailwind CSS，响应式设计
- 📱 **移动端友好** - 完美适配各种设备，支持触摸滑动
- 🎨 **作品集展示** - AI项目、设计作品、实习经验
- 🎭 **动画效果** - 使用Framer Motion，流畅的交互体验
- 🔧 **易于维护** - 模块化组件，清晰的代码结构

## 🏗️ 技术栈

- **前端框架**: React 18.3.1 + TypeScript
- **构建工具**: Vite 6.3.5
- **样式框架**: Tailwind CSS
- **动画库**: Framer Motion
- **包管理**: npm
- **部署**: GitHub Pages + GitHub Actions

## 📊 网站内容

### AI Coding Portfolio
- 个人网站模板项目
- 展示React、TypeScript等前端技术

### Design Portfolio
- 荔枝采摘机器人（工业设计、机械结构、农业）
- 酒店行李寄送服务设计（服务设计、概念设计、环保理念）
- 荔枝认养系统设计（系统设计、服务设计、农业）
- 儿童粤语学习机（工业设计、儿童早教、文化创意）
- 六神音乐节-品牌策划案（品牌营销、活动策划、方案设计）

### Intern Experience
- **美团** (2024.06-2024.09) - AI产品经理
- **TCL** (2025.03-2025.05) - AI产品经理
- **文石** (2024.01-2024.05) - 产品经理
- **荣耀** (2024.05-2024.12) - 用户体验优化项目

## 🚀 快速开始

### 1. 克隆项目
```bash
git clone https://github.com/eatingwang012/eatingwang012.github.io.git
cd eatingwang012.github.io
```

### 2. 安装依赖
```bash
npm install
```

### 3. 启动开发服务器
```bash
npm run dev
```

访问 http://localhost:3000 查看效果

### 4. 构建生产版本
```bash
npm run build
```

## 📁 项目结构

```
src/
├── components/          # 可复用组件
│   ├── Navigation.tsx   # 导航栏组件
│   ├── PortfolioCard.tsx # 项目卡片组件
│   ├── ProjectModal.tsx # 项目详情模态框
│   ├── ExperienceCard.tsx # 经验卡片组件
│   └── Empty.tsx        # 空状态组件
├── pages/               # 页面组件
│   ├── Home.tsx         # 首页
│   ├── AiPortfolio.tsx    # AI作品集
│   ├── ArchitecturePortfolio.tsx # 设计作品集
│   └── Experience.tsx   # 经验页面
├── data/                # 数据文件
│   ├── personal.ts      # 个人信息
│   ├── aiProjects.ts    # AI项目数据
│   ├── architectureProjects.ts # 设计项目数据
│   ├── experiences.ts   # 经验数据
│   └── profileImages.ts # 头像图片
├── contexts/            # React上下文
├── hooks/               # 自定义钩子
└── lib/                 # 工具函数
```

## 🚀 部署

### GitHub Pages 自动部署
项目使用GitHub Actions自动部署到GitHub Pages：

1. 推送代码到main分支
2. GitHub Actions自动构建和部署
3. 网站自动更新到 https://eatingwang012.github.io

### 手动部署
```bash
npm run build
npm run deploy
```

## 🎨 自定义

### 修改个人信息
编辑 `src/data/personal.ts` 文件，更新个人信息。

### 修改项目数据
- AI项目：编辑 `src/data/aiProjects.ts`
- 设计项目：编辑 `src/data/architectureProjects.ts`
- 工作经验：编辑 `src/data/experiences.ts`

### 修改样式
编辑 `tailwind.config.js` 或 `src/index.css` 来自定义样式。

## 📝 注意事项

1. **图片资源**: 确保所有图片都在 `public/` 目录下
2. **移动端优化**: 项目已优化移动端触摸体验
3. **SEO优化**: 已配置基本的SEO元标签
4. **性能优化**: 使用Vite构建，支持代码分割

## 🌐 访问网站

**在线预览**: https://eatingwang012.github.io

## 📄 许可证

本项目采用 MIT 许可证

## 🙏 致谢

感谢所有为这个项目提供帮助的朋友们！

---

**联系方式**: eatingwang012@163.com
