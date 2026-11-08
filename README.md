# 我的技术文档（my-docs）

使用 MkDocs Material 搭建的个人静态文档网站，通过 GitHub Actions 自动构建并部署到 GitHub Pages。

- 网站地址：https://Liuziyu0714.github.io/my-docs/
- 实验报告：[个人实验报告](report/README.md)

## 本地预览

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m mkdocs serve
```

浏览器打开 `http://127.0.0.1:8000/` 预览，按 `Ctrl+C` 停止。

## 目录说明

| 路径 | 说明 |
| --- | --- |
| `docs/` | 文档源码（Markdown） |
| `mkdocs.yml` | MkDocs 站点配置与导航 |
| `.github/workflows/deploy.yml` | 推送 main 后自动构建并部署到 Pages |
| `report/` | 实践过程报告与截图 |
| `site/` | 构建产物（已 gitignore，由 Actions 生成） |
