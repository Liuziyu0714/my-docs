# 使用指南

1. 修改 docs 目录中的 Markdown 文件。
2. 在本地预览并检查页面及链接。
3. 提交修改并推送到 main 分支。
4. 在 Actions 页面查看构建与部署状态。
5. 打开网站检查内容是否更新。

## 常用命令

- `python -m mkdocs serve`：本地预览。
- `python -m mkdocs build --strict`：构建网站并严格检查警告。

## 本地环境搭建示例

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m mkdocs serve
```

执行后在浏览器打开 `http://127.0.0.1:8000/` 即可预览，按 `Ctrl+C` 停止。

## 推送后如何确认部署

推送后不要手动重新运行工作流，先到仓库的 Actions 页面确认这次 push 自动触发了新的运行，等待 build 和 deploy 两个任务都变绿后，强制刷新（或使用无痕窗口）打开网站核对新内容。返回[首页](index.md)。
