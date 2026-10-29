# 帧刻 FRAME

视频剪辑 App 介绍页面，页脚包含「上海帧溯科技有限公司」。

## GitHub Pages

1. 把此目录的文件推送到 GitHub 仓库的 `main` 分支，包括 `.github/workflows/pages.yml`。
2. 在仓库的 **Settings → Pages → Build and deployment** 中，将 **Source** 设为 **GitHub Actions**。
3. 在 **Actions → Deploy FRAME to GitHub Pages → Run workflow** 手动启动一次部署。后续推送到 `main` 会自动更新。
4. 等待部署成功，在 **Settings → Pages** 获取网站地址。

页面文件放在 `site/` 下，无需安装依赖或构建。相对路径适配 GitHub Pages 的仓库子路径。

## 本地预览

```sh
python3 -m http.server 8080 --directory site
```

然后访问 `http://localhost:8080`。

当前为产品概念展示，交互预览使用静态图片，不支持处理或导出真实视频。图片来自 Pexels，字体通过 Google Fonts 加载。
