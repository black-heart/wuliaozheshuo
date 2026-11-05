# 无聊者说

一组轻松、缓慢的小体验。网站是纯静态页面，不需要服务器或数据库。

## GitHub Pages 部署

仓库已配置 GitHub Actions：将改动推送到 `main` 后，会自动发布 `dist/` 目录。

首次发布时，在 GitHub 仓库打开 **Settings → Pages**，将 **Build and deployment → Source** 设为 **GitHub Actions**。等待 Actions 中 `Deploy to GitHub Pages` 工作流成功后，地址为：

`https://<GitHub 用户名>.github.io/<仓库名>/`

也可以在 **Settings → Pages → Custom domain** 里添加自己的域名。绑定域名需要在域名 DNS 中按 GitHub 提示添加记录。

## 本地预览

直接打开 `dist/index.html`，或在项目根目录运行：

```sh
python3 -m http.server 8000 --directory dist
```

## 内容

- `dist/index.html`：页面结构和中文内容
- `dist/style.css`：布局、配色和响应式样式
- `dist/app.js`：木鱼、青蛙、燃香、蜗牛与蚂蚁互动
