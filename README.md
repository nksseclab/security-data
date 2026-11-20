# VulnData 静态展示页

纯 HTML / CSS / JavaScript，无构建依赖。支持手机布局、四类案例切换、键盘切换标签及 JSON/CSV 下载。品牌名 VulnData 是样板名称，可自行替换。

## 本地查看

直接打开 `index.html`，或在本目录运行 `python -m http.server 8080`，访问 http://localhost:8080 。

## GitHub Pages

1. 新建 GitHub 仓库，把**本文件夹内的内容**上传到仓库根目录。
2. 在仓库 Settings → Pages 中选择 Deploy from a branch。
3. 选择 main 分支、/(root)，保存后等待部署完成。

所有资源使用相对路径，可部署在 `用户名.github.io/仓库名/`。无需服务器、数据库或 API 密钥。Google Fonts 为可选外部字体，加载失败时自动使用本机字体。

## 修改内容

- `index.html`：规模、指标、资源介绍及下载入口。
- `style.css`：配色、布局和响应式样式。
- `app.js`：四类案例的加工前后内容与交互。
- `data/`：可下载的局部数据节选及任务目录。

## 数据依据

漏洞规模和 VINCI 指标来自已有论文材料；PoC 和 Patch 指标来自“四类数据”内介绍及 CSV；评测目录来自 bench_all.csv。不同研究的样本与指标不直接比较。PoC 总量按“51 万+”展示以兼容两个快照；题目数不等于独立 CVE 数。

漏洞 JSON 是实际结果的局部节选，不是完整验证后的权威漏洞记录。下载数据保留各原来源的权利，第三方再分发范围应依其许可。本目录不包含完整第三方数据库或评测题包。

页面为新编写的独立实现，未复制 Academic Project Page 或 Tabler 的模板代码。
