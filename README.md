# 游戏日历 (Game Calendar)

加载 ICS 文件，展示游戏活动日历。

## 功能特性

- 📅 支持加载标准 `.ics` 日历文件（本地文件或远程 URL）
- 🎮 专为游戏活动（副本、活动、卡池等）设计
- 🔄 自动解析事件标题、时间、描述
- 🧰 操作按钮：支持 `重置` / `导入` / `导出` 删除记录
- 🔗 可通过 URL 或本地文件加载 ICS 订阅
- 🌐 纯静态，可直接在浏览器中打开使用

## TODO

- 查找燕云十六声游戏活动ics日历

## 使用说明

1. 直接打开 `index.html` 即可在浏览器中查看日历。
2. 右键点击事件可删除，删除记录会保存在浏览器 cookie 中。
3. 点击 `导出` 可导出当前删除事件列表，点击 `导入` 可恢复之前导出的删除记录。
4. 点击 `重置` 可清除已删除记录并刷新页面。

## 目录结构

- `index.html` — 主日历页面
- `ics/` — 本地 ICS 文件目录，包含各游戏活动源
- `js/` — 第三方库文件，如 `daypilot-all.min.js` 和 `ical.min.js`
- `.github/workflows/update-ics.yml` — 每周自动下载 ICS 的 GitHub Action

## 主要依赖

- **日历组件**：[DayPilot](https://code.daypilot.org/)
- **ICS 解析**：[ical.js](https://github.com/mozilla-comm/ical.js)
- **数据源示例**：[hoyo_calendar](https://github.com/Trrrrw/hoyo_calendar)

## GitHub Action

工作流文件位于 `.github/workflows/update-ics.yml`，负责每周下载三份远程 ICS 文件并提交到仓库。

## 运行方式

- 本地：直接用浏览器打开 `index.html`
- 远程：将仓库部署到静态站点或 GitHub Pages 即可访问