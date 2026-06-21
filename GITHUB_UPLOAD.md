# GitHub 上传步骤

## 1) 新建仓库

在 GitHub 创建一个空仓库（不要勾选 README / .gitignore / License）。

## 2) 本地初始化并提交

```bash
cd Deepscape_Reverie_Web_release
git init
git add .
git commit -m "chore: initial release of Deepscape Reverie"
```

## 3) 关联远程并推送

把下面 URL 换成你的仓库地址：

```bash
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## 4) 常见问题

1. 如果推送失败提示文件过大：
   - 先执行 `git status` 确认是否误加了额外大文件。
   - 本项目精简版当前约 77MB，单文件均低于 GitHub 100MB 限制。

2. 如果页面打开空白：
   - 确认 `index.html` 与 `知识图谱/20260130知识图谱.html` 路径未改。

3. 如果 GitHub Pages 部署：
   - 进入仓库 `Settings -> Pages`
   - Source 选 `GitHub Actions`
   - 推送到 `main` 后，`.github/workflows/pages.yml` 会自动发布根目录网页
   - 入口地址为 `https://610lulu.github.io/Deepscape-Reverie/`
