# 关于本项目

## 项目目标

实现从 Markdown 文档到公开网站的自动化发布：每次向 main 分支推送文档修改，GitHub Actions 都会自动重新构建并部署网站。

## 技术组成

| 工具 | 作用 |
| --- | --- |
| Markdown | 编写文档内容 |
| MkDocs Material | 将文档构建成静态网站 |
| GitHub Actions | 自动执行安装、构建和部署 |
| GitHub Pages | 托管并提供网站访问地址 |

## 我的工作流理解

`docs/` 目录存放的是源码，`site/` 目录是 `mkdocs build` 生成的产物。产物不需要手工维护——GitHub Actions 在云端重新执行构建，并通过 `actions/upload-pages-artifact` 把 `site/` 上传为 Pages 制品，最后由 `actions/deploy-pages` 发布。因此本地或远程都不需要提交 `site/`，它已被加入 `.gitignore`。

更多操作步骤见[使用指南](guide.md)，接口示例见[API 参考](api.md)。
