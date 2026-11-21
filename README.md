# 网站结构

- `index.html`：外壳（样式、菜单、搜索、主页、圣经软件下载页）。平时不用改。
- `content/manifest.json`：内容清单，决定加载哪些文件、按什么顺序。
- `content/verses.html`：圣经经文页。
- `content/fragments.html`：镜鉴·零言（每次加一句，改这个文件）。
- `content/notes/note-N.html`：随读笔记，一篇一个文件。
- `content/essays/essay-N.html`：镜鉴·篇章，一篇一个文件。

## 新增一篇笔记
1. 复制一个现有的 `content/notes/note-N.html`，改名为下一个编号（如 `note-11.html`），里面的 `id="page-note-11"` 也改成同样编号，再改标题和正文。
2. 在 `content/manifest.json` 的 `"notes"` 列表末尾加一行 `"content/notes/note-11.html"`。篇章同理。

## 注意
网站必须通过网址（GitHub Pages）访问；直接双击本地的 index.html 无法加载内容。
