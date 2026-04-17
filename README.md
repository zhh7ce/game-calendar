# 游戏日历 (Game Calendar)

加载 ICS 文件，展示游戏活动日历。

## 功能特性

- 📅 支持加载标准 `.ics` 日历文件（本地文件或远程 URL）
- 🎮 专为游戏活动（副本、活动、卡池等）设计
- 🔄 自动解析事件标题、时间、描述
- 🖥️ 简洁的日历视图，支持按日/周/月展示
- 🔗 可通过 URL 或本地文件加载 ICS 订阅
- 🌐 纯静态，可直接在浏览器中打开使用

## 主要依赖

- **日历组件**：[DayPilot](https://code.daypilot.org/)
- **ICS 解析**：[ical.js](https://github.com/mozilla-comm/ical.js)
- **数据源示例**：[hoyo_calendar](https://github.com/Trrrrw/hoyo_calendar)