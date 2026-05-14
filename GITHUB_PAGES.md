# GitHub Pages 发布说明

这个项目是纯静态 HTML，可以直接使用 GitHub Pages 发布。

## 第一步：创建 GitHub 仓库

仓库名建议：

```text
open-llm-app-roadmap
```

## 第二步：推送代码

在本项目目录下执行：

```bash
git init
git add .
git commit -m "Initial roadmap site"
git branch -M main
git remote add origin https://github.com/<your-username>/open-llm-app-roadmap.git
git push -u origin main
```

把 `<your-username>` 替换成你的 GitHub 用户名。

## 第三步：开启 GitHub Pages

进入仓库页面：

```text
Settings → Pages
```

选择：

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

点击保存。

## 第四步：访问站点

构建完成后，访问：

```text
https://<your-username>.github.io/open-llm-app-roadmap/
```

## 常见问题

### 页面样式没有加载

确认仓库根目录中存在：

```text
styles.css
```

并且 `index.html` 中引用的是：

```html
<link rel="stylesheet" href="styles.css">
```

### 子页面打不开

确认每个阶段目录下都有：

```text
index.html
```

例如：

```text
04-rag/index.html
```

### GitHub Pages 没有更新

GitHub Pages 可能需要等待几十秒到几分钟。也可以在仓库的 `Actions` 或 `Pages` 页面查看构建状态。
