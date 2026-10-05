# CRM English Work Simulator

移动端优先的 CRM / 海外运营英语听力训练 MVP。第一批题库覆盖 CRM Ops、Lifecycle、Campaign、Experiment 和 AI automation，内置 stakeholder、operational request、KYC、FTD、FTT、control group、statistical significance 等面试业务表达。

## 运行

1. 安装 Node.js 20+。
2. 在项目目录运行 `npm install`。
3. 运行 `npm run dev` 并打开终端显示的地址。
4. 生产构建：`npm run build`。

## 使用

- 今日训练：无字幕听音，填写关键词和六要素（Audience / Objective / Trigger / Channel / Action / KPI）。
- 首次未达标只显示提示，第二次提交后展示原文、中文业务意思、词块和复盘。
- 会议模拟：听需求会并提交摘要、澄清问题。
- 我的弱项：在当前浏览器本地保存训练分数与漏听词块，自动聚合高频弱项。

## 音频与后续迁移

默认使用浏览器免费 Web Speech API，无需 API key；推荐 Chrome 或 Edge。若需接真实录音或第三方 TTS，只要替换 `src/main.jsx` 的 `speak()` 即可；题库结构和页面逻辑可复用。迁移到微信小程序时，将语音播放、页面壳与本地存储替换成小程序等价 API 即可。
