# HR · AI 需求自测问卷

一个纯静态的单页问卷，用于 HR 团队快速评估「是否适合引入 AI / 从哪个场景切入」。全部逻辑与样式内联在单个 HTML 文件中，无任何外部依赖。

## 在线访问

部署在 GitHub Pages，仓库 Settings → Pages 中查看当前站点地址。

## 本地预览

直接用浏览器打开 `index.html` 即可，无需构建、无需服务器。

## 目录结构

```
index.html                    # 发布入口（GitHub Pages 使用）
.nojekyll                     # 关闭 Jekyll 处理，按原样托管
dist/AI自测需求.html          # 内容源文件（与 index.html 一致）
dist/index.html               # 历史入口（已由根目录 index.html 取代）
```

## 更新网页内容

替换 `dist/AI自测需求.html` 后，执行：

```bash
cp "dist/AI自测需求.html" index.html
git add -A && git commit -m "Update questionnaire" && git push
```

GitHub Pages 会在约 1 分钟后自动重新构建。
