# Darkatse's blog

[darkatse.com](https://darkatse.com)

基于 [Yihui Xie 的 Hugo Paged](https://github.com/yihui/hugo-paged)，保留主题的示例文章供后续修改。

## 本地预览

```sh
hugo server
```

文章放在 `content/blog/`，首页为 `content/_index.md`，站点设置在 `hugo.yaml`。

## 部署

Cloudflare Pages 项目 `darkatse-blog` 连接本仓库，推送到 `main` 后自动构建并部署到 `darkatse.com`。
其他分支会生成预览地址，便于发布前检查。

- Hugo：`0.166.0`（Pages 环境变量 `HUGO_VERSION`）
- 构建命令：`hugo --gc --minify`
- 输出目录：`public`
