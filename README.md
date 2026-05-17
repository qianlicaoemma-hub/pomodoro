# Pomodoro · A Focus Instrument

一个单文件 HTML 番茄钟，桌面双击即用，无需安装，无需联网。

设计风格：编辑设计 / 意大利老式年鉴 —— 奶油纸底、墨黑、番茄红。

## 使用

直接双击 `index.html`，或在浏览器中打开。

## 功能

- 三种模式：Focus 25 min · Pause 5 min · Recess 15 min
- 横向刻度进度条（每分钟一格，每 5 格加粗）
- 完成专注后：声音提醒 + 系统通知 + 红色印章动画 + 今日计数 +1
- 今日完成数本地存储（`localStorage`，按日期）

## 快捷键

| 键 | 作用 |
| --- | --- |
| `Space` | 开始 / 暂停 |
| `R` | 重置当前阶段 |
| `1` `2` `3` | 切换 Focus / Pause / Recess |

## 技术

- 单个 HTML 文件，无依赖、无构建
- 字体：Fraunces（display）+ IBM Plex Mono（utility），通过 Google Fonts 加载
- 声音：Web Audio API 现场合成
- 通知：浏览器 Notifications API（首次使用授权一次即可）
