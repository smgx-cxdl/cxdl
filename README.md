# 网站结构（所有文件都在最外层）

- index.html：外壳（样式、菜单、搜索、主页、下载页），平时不用改
- manifest.json：内容清单，决定加载哪些文件、按什么顺序
- verses.html：圣经经文；fragments.html：镜鉴·零言
- note-N.html：随读笔记，一篇一个文件；essay-N.html：篇章，一篇一个文件

新增一篇笔记：复制一个 note-N.html，改名为下一个编号（如 note-11.html），把里面的 id="page-note-11"、标题和正文改掉，再在 manifest.json 的 "notes" 里加一行 "note-11.html"。
网站必须通过网址访问，直接双击 index.html 无法加载内容。
