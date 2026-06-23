# TokenDirect — 企业级 AI Token 服务站点

一个 Apple 风格的双语（中 / EN）静态站点，由两个页面组成：

| 文件 | 角色 | 说明 |
| --- | --- | --- |
| `index.html` | 主页 | TokenDirect 商业落地页：风险 → 方案 → 对比 → 架构 → 联系 |
| `relay-risks.html` | 深度解析 | 「中转站到底会不会存你的数据」技术与信任模型分析长文 |

两页共用同一套设计系统（Inter + Noto Sans SC 字体、`#0071e3` 主色、统一导航与页脚），并相互链接：主页「风险」区块导向深度文章，文章结尾导回方案。

## 本地预览

直接用浏览器打开 `index.html` 即可，无需任何构建或依赖（仅通过 CDN 引入 Google Fonts）。

## 部署到 GitHub Pages

1. 新建一个仓库（例如 `tokendirect-site`），把本文件夹内所有文件上传到仓库根目录。
2. 进入仓库 **Settings → Pages**。
3. **Source** 选择 `Deploy from a branch`，**Branch** 选择 `main`（或 `master`）、目录选 `/ (root)`，保存。
4. 等待约 1 分钟，页面会显示你的站点地址，形如：
   `https://<你的用户名>.github.io/tokendirect-site/`
5. 访问该地址即为主页；深度文章在 `.../relay-risks.html`。

> 如果想让站点地址不带仓库名（即 `https://<用户名>.github.io/`），把仓库命名为 `<你的用户名>.github.io` 即可。

## 文件结构

```
tokendirect-site/
├── index.html         # 主页
├── relay-risks.html   # 深度解析文章
└── README.md
```

## 备注

- 双语切换：点击导航右上角 `EN / 中` 按钮，可隐藏 / 显示英文。
- 内容中的风险分析基于公开资料，仅供参考，不针对任何具体平台。
- 联系邮箱等占位信息（`contact@example.com`）请按需替换。
