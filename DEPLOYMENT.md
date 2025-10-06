# 🚀 GitHub Pages 部署指南

## 📋 部署步骤

### 1. 创建GitHub仓库

1. **登录GitHub**
   - 访问 https://github.com
   - 使用您的账号 `eatingwang012@163.com` 登录

2. **创建新仓库**
   - 点击右上角的 "+" 号，选择 "New repository"
   - 仓库名称：`eatingwang012.github.io`（必须使用这个名称）
   - 描述：`个人作品集网站`
   - 选择 "Public"（公开仓库）
   - 不要勾选 "Add a README file"（我们已经有了）
   - 点击 "Create repository"

### 2. 上传代码到GitHub

#### 方法A：使用Git命令行（推荐）

```bash
# 1. 初始化Git仓库（如果还没有）
git init

# 2. 添加所有文件
git add .

# 3. 提交更改
git commit -m "Initial commit: Personal portfolio website"

# 4. 添加远程仓库
git remote add origin https://github.com/wangyiting0412/eatingwang012.github.io.git

# 5. 推送到GitHub
git branch -M main
git push -u origin main
```

#### 方法B：使用GitHub Desktop

1. 下载并安装 GitHub Desktop
2. 选择 "Clone a repository from the Internet"
3. 输入仓库URL：`https://github.com/eatingwang012/eatingwang012.github.io.git`
4. 选择本地文件夹
5. 将项目文件复制到克隆的文件夹中
6. 在GitHub Desktop中提交并推送更改

### 3. 启用GitHub Pages

1. **进入仓库设置**
   - 在您的GitHub仓库页面，点击 "Settings" 标签

2. **配置Pages**
   - 在左侧菜单中找到 "Pages"
   - 在 "Source" 部分选择 "GitHub Actions"
   - 保存设置

3. **等待自动部署**
   - GitHub Actions会自动开始构建和部署
   - 您可以在 "Actions" 标签页查看部署进度
   - 部署完成后，网站将在 `https://eatingwang012.github.io` 可用

### 4. 验证部署

1. **检查部署状态**
   - 访问 https://eatingwang012.github.io
   - 如果看到您的个人网站，说明部署成功

2. **检查Actions状态**
   - 在GitHub仓库的 "Actions" 标签页
   - 确保所有工作流都显示绿色（成功）

## 🔧 本地开发

### 启动开发服务器
```bash
# 使用完整路径运行npm
& "E:\nodeJS\npm.cmd" run dev
```

### 构建生产版本
```bash
# 构建项目
& "E:\nodeJS\npm.cmd" run build

# 预览构建结果
& "E:\nodeJS\npm.cmd" run preview
```

## 📝 更新网站内容

### 修改个人信息
编辑 `src/data/personal.ts` 文件：
```typescript
export const personalInfo = {
  name: "王亦婷",
  position: "Tina Wang",
  // ... 其他信息
};
```

### 添加新项目
编辑 `src/data/aiProjects.ts` 或 `src/data/architectureProjects.ts`：
```typescript
export const aiProjects = [
  {
    id: 4,
    title: "新项目标题",
    description: "项目描述",
    imageUrls: ["/new-project.jpg"],
    tags: ["新标签"],
    githubUrl: "https://github.com/yourusername/project"
  }
];
```

### 更新工作经历
编辑 `src/data/experiences.ts`：
```typescript
export const experiences = [
  {
    id: 4,
    title: "新职位",
    company: "新公司",
    period: "2024-2025",
    // ... 其他信息
  }
];
```

## 🚀 自动部署流程

每次您推送代码到main分支时：

1. **GitHub Actions自动触发**
   - 自动安装依赖
   - 自动构建项目
   - 自动部署到GitHub Pages

2. **部署时间**
   - 通常需要2-5分钟完成部署
   - 可以在Actions页面查看进度

3. **访问网站**
   - 部署完成后，访问 https://eatingwang012.github.io
   - 网站会自动更新为最新版本

## 🛠️ 故障排除

### 常见问题

1. **网站无法访问**
   - 检查GitHub Pages是否已启用
   - 确认仓库名称为 `eatingwang012.github.io`
   - 等待几分钟让DNS生效

2. **构建失败**
   - 检查Actions页面的错误日志
   - 确保所有依赖都已正确安装
   - 检查代码是否有语法错误

3. **图片无法显示**
   - 确保图片文件在 `public/` 目录下
   - 使用 `/filename.jpg` 格式引用图片
   - 检查文件名大小写是否正确

### 获取帮助

如果遇到问题：
1. 查看GitHub Actions的日志
2. 检查GitHub Pages的设置
3. 确认仓库权限设置正确

## 📞 联系信息

- GitHub: https://github.com/eatingwang012
- 邮箱: eatingwang012@163.com

---

**部署完成后，您的个人网站将在 https://eatingwang012.github.io 上线！**
