# 我的技术文档

欢迎访问我的个人文档网站。本网站使用 MkDocs 构建，通过 GitHub Actions 自动部署到 GitHub Pages。

- 作者：Liuziyu0714
- 实践主题：静态文档自动部署
- [关于本项目](about.md)
- [使用指南](guide.md)
- [API 参考](api.md)

## 实践简介

这是我完成的"02-github-pages"实践项目：从零搭建一个 MkDocs 文档网站，并通过 GitHub Actions 实现"推送代码 → 自动构建 → 自动部署 → 网站更新"的完整流程。整个过程不需要手动创建 gh-pages 分支，也不需要手动上传构建产物，全部由官方 Pages 工作流完成。

通过本次实践，我理解了源码（docs/）、构建产物（site/）、工作流（deploy.yml）和托管服务（GitHub Pages）四者之间的关系，并学会了通过 Actions 日志排查部署问题。

自动部署验证：这是我第二次推送后更新的内容。
