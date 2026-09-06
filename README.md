# 嵌入式作品集

单页作品集，展示王琨的三个嵌入式项目：自平衡小车、FreeRTOS+LVGL 示波器、Linux+Qt 车载副屏。页面为纯 HTML/CSS/JS，不需要安装依赖。

## 目录结构

```text
作品集/
├── index.html
├── README.md
├── .nojekyll
├── assets/js/lucide.min.js
└── images/
```

## 替换自己的资料

1. 把真实照片、视频截图、原理图放到 `images/` 文件夹。
2. 编辑 `index.html`：
   - 顶部姓名、电话、邮箱、城市改成真实信息。
   - 项目里的内联 SVG 示意可换成 `<img src="images/xxx.jpg" alt="项目图">`。
   - 每个项目按钮的 `href="#"` 换成 GitHub 仓库、演示视频、设计文档链接。
3. 保存后用浏览器打开 `index.html` 预览。

## 发布到 GitHub Pages

1. 在 GitHub 创建一个公开仓库，例如 `portfolio`。
2. 在本文件夹执行：

```powershell
git init -b main
git add .
git commit -m "初始化作品集"
git branch -M main
git remote add origin https://github.com/你的用户名/portfolio.git
git push -u origin main
```

3. 在仓库网页打开 `Settings -> Pages`，Source 选择 `Deploy from a branch`，分支选择 `main`，目录选择 `/ (root)`，保存。
4. 等 1-2 分钟后访问：`https://你的用户名.github.io/portfolio/`。

## 注意

- 图标文件已本地化到 `assets/js/lucide.min.js`，发布后不依赖外部 CDN。
- 页面本身是公开的，不要上传带密钥、账号密码的文件。
- 后续更新资料后执行 `git add . && git commit -m "更新" && git push` 即可。
