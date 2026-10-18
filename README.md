# TQSY's Space

个人主页 / 链接集合站。单页，无后端。

## 结构

站点只有一个页面 `src/pages/index.astro`，HTML、CSS、JS 全部内联，不依赖任何组件或集成；
`src/pages/404.astro` 是独立的 404 页，同样不依赖主题文件。

## 命令

```bash
npm install      # 依赖只有 astro + prettier
npm run dev      # http://localhost:4321
npm run build    # 输出到 dist/
npm run preview  # 预览构建产物
```

## 部署

Cloudflare Pages，连 `main` 分支自动构建（构建命令 `npm run build`，输出目录 `dist`）。

## 说明

- 站内图片与音频走外部托管（catbox / videotourl），不在仓库里
- 依赖只有 `astro`，没有 Tailwind、没有 MDX、没有搜索索引
