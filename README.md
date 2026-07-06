# 申聆空间设计 — BRUTALIST EDITION

粗犷设计风格的第二版作品集网站。

## 部署到 GitHub Pages

1. 在 GitHub 创建仓库（如 `username/portfolio-brutalist`）
2. 推送本项目到 `main` 分支
3. Settings → Pages → Source 选 `main` 分支
4. 网站将在 `https://username.github.io/portfolio-brutalist/` 上线

## 与第一版的区别

| 特性 | 第一版（极简高端） | 第二版（粗犷设计） |
|------|------------------|-------------------|
| 配色 | 白/米白/炭灰/暖金 | 橙/青/黄/黑/白 |
| 字体 | Playfair Display + Inter | Space Mono + IBM Plex Sans |
| 边框 | 无边框 | 3-4px 黑色实线 |
| 阴影 | 柔和渐变 | 硬边色块阴影 |
| 图片 | 彩色展示 | hover 黑白→彩色 |
| 按钮 | 描边透明 | 实心色块+硬阴影 |
| 弹窗 | 右侧滑出白底 | 右侧滑出黑底+青色 |
| 内容 | 完全一致 | 完全一致（仅风格不同） |

## 自定义指南

### 替换图片
将 `images/` 目录下的占位图替换为真实图片，文件名保持一致：
- `images/hero-bg.jpg` — 首页背景（1920×1080）
- `images/about-me.jpg` — 个人照片（800×1000）
- `images/portfolio/project-*.jpg` — 项目封面（1200×800）

### 修改文案
- 页面文字 → `index.html`
- 弹窗详情 → `js/main.js` 中的 `projects` 对象

### 修改配色
`css/style.css` 顶部的 `:root` 变量：
```css
:root {
  --orange:   #FF6B35;  /* 主色 */
  --cyan:     #00F0FF;  /* 强调色 */
  --yellow:   #FFE600;  /* 点缀色 */
  /* ... */
}
```
