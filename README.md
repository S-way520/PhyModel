# PhyModel 官方网站

物理模型 (PhyModel) - AI驱动的交互式物理学习平台官方网站

## 部署到 GitHub Pages

### 方法一：通过 GitHub 网页界面

1. 在 GitHub 上创建一个新仓库（或使用现有仓库）
2. 将所有文件上传到仓库根目录：
   - `index.html`
   - `privacy.html`
   - （可选）`app-icon.png` - 如果希望显示网站图标
3. 进入仓库的 **Settings** → **Pages**
4. 在 **Source** 部分选择：
   - **Branch**: `main` (或 `master`)
   - **Folder**: `/ (root)`
5. 点击 **Save**
6. 等待几分钟，GitHub Pages 会自动生成网站链接
7. 访问链接：`https://你的用户名.github.io/仓库名/`

### 方法二：通过 Git 命令行

```bash
# 初始化 Git 仓库（如果还没有）
git init

# 添加所有文件
git add .

# 提交
git commit -m "Initial commit: PhyModel website"

# 添加 GitHub 远程仓库
git remote add origin https://github.com/你的用户名/仓库名.git

# 推送到 GitHub
git branch -M main
git push -u origin main
```

然后在 GitHub 仓库设置中启用 Pages（步骤同方法一）。

## 注意事项

- **app-icon.png**: 代码中引用了这个图标文件，如果不存在，浏览器会显示默认图标，但不影响网站功能。如需添加，请将图标文件放在根目录。
- **相对路径**: 所有链接都使用相对路径，适合 GitHub Pages 部署。
- **HTTPS**: GitHub Pages 自动提供 HTTPS 支持。

## 文件结构

```
/
├── index.html          # 主页
├── privacy.html        # 隐私协议页面
└── app-icon.png        # 网站图标（可选）
```

## 自定义域名（可选）

如果需要使用自定义域名：

1. 在仓库根目录创建 `CNAME` 文件
2. 在文件中写入你的域名，例如：`www.yourdomain.com`
3. 在你的域名 DNS 设置中添加 CNAME 记录指向 `你的用户名.github.io`

