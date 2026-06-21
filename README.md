# Deepscape Reverie

深景迴梦（Deepscape Reverie）静态网页项目，包含主站页面与访谈知识图谱子页面。

## Live Site

https://610lulu.github.io/Deepscape-Reverie/

## 目录结构

```text
Deepscape_Reverie_Web_release/
├─ index.html                  # 主页面
├─ assets/                     # 主站图片资源
├─ 知识图谱/
│  ├─ 20260130知识图谱.html     # 图谱页面
│  └─ images/                  # 图谱页面使用的图片
├─ docs/
│  └─ site-improvement-plan.md # 站点优化计划文档
└─ .gitignore
```

## Notes

- 图谱页面由 `index.html` 通过 iframe 引用：`知识图谱/20260130知识图谱.html`。
- 如果调整目录名（尤其是 `知识图谱`），请同步修改 `index.html` 中的 iframe 路径。
