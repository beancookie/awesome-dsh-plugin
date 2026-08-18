<p align="center">
  <a href="https://beancookie.github.io/awesome-dsh-plugin/zh/">
    <img src="https://beancookie.github.io/awesome-dsh-plugin/logo.png" alt="Awesome DSH Plugin" width="120">
  </a>
</p>

# Awesome DeepSeek Harness (DSH) Plugin

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="https://beancookie.github.io/awesome-dsh-plugin"><img src="https://beancookie.github.io/awesome-dsh-plugin/badge.svg" alt="awesome · DSH plugin"></a>
</p>

<p align="center">
  <a href="README.en.md">English</a> | 中文
</p>

> [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness)（`dsh`）插件精选列表。

DeepSeek Harness 是 DeepSeek 开源的 agent harness——既是可直接运行的 Coding Agent（提供 Web 与 headless 两种形式），底层又是一套「一切皆插件」的框架：模型、工具、沙箱、会话存储、UI、乃至 Agent Loop 本身都是插件。插件既可以扩展官方 Coding Agent，也可以替换其核心部件，甚至组装出完全不同的东西。

<p align="center">
  推荐使用 <a href="https://github.com/beancookie/dsh-plugin-registry">dsh-plugin-registry</a> —— 会话内检索并一键安装本列表插件，Web 设置页带「插件市场」面板。
</p>

<details>
<summary align="center">📸 点击查看演示截图</summary>

<p align="center">
  <img src="images/dsh-plugin-registry.png" alt="dsh-plugin-registry" width="600">
</p>

</details>

**373** 个插件 · 欢迎 [PR](#贡献)

## 目录

- [插件](#插件)
  - [🎨 UI 增强](#-ui-增强)
  - [🎭 主题与外观](#-主题与外观)
  - [💬 会话与消息](#-会话与消息)
  - [🧠 记忆](#-记忆)
  - [🛠️ 工具与能力](#-工具与能力)
  - [🧩 技能包](#-技能包)
  - [🔁 工作流与自动化](#-工作流与自动化)
  - [🔔 通知与集成](#-通知与集成)
  - [🔌 模型与账号接入](#-模型与账号接入)
  - [🧑‍💻 开发与运行时](#-开发与运行时)
  - [🎮 娱乐](#-娱乐)
- [相关](#相关)
- [贡献](#贡献)
- [徽章](#徽章)
- [免责声明](#免责声明)

## 插件

### 🎨 UI 增强
- [0xsline/dsh-spotlight](https://github.com/0xsline/dsh-spotlight) — 键盘优先的命令面板（command palette）。
- [a903067276-rgb/dsh-file-mentions](https://github.com/a903067276-rgb/dsh-file-mentions) — DSH 回复中的文件路径可点击：Codex 风格行内打开、文件管理器定位、回合尾部文件 chip 列表。
- [a903067276-rgb/dsh-hud](https://github.com/a903067276-rgb/dsh-hud) — HUD 状态面板：Git 状态、MCP 服务器、技能列表、模型与 token 用量，悬浮侧栏一览无余。
- [AKIRACOD/dsh-drag-and-drop](https://github.com/AKIRACOD/dsh-drag-and-drop) — 拖放 fork：文档以可删除「文件芯片」挂在输入框上方，不打字也能发送。
- [alingalingling/ui-status-label](https://github.com/alingalingling/ui-status-label) — 把鲸鱼娘思考时的 "deep diving" 状态文案自定义成任意你想要的样子。
- [asukasec/dsh-message-preview](https://github.com/asukasec/dsh-message-preview) — 右侧用户消息导航条，根据消息数量与可用高度自适应排布导航块，并支持悬停预览、键盘操作与点击跳转。
- [BeiZi6/dsh-opencodego-usage](https://github.com/BeiZi6/dsh-opencodego-usage) — OpenCodeGo 剩余额度监视器：输入框右下角呼吸指示灯（按剩余额度绿/黄/红），液态玻璃面板显示滚动/周/月用量窗口与重置时间，每 30 秒自动刷新，API Key 自动读取 DSH 凭据。
- [bill9109/dsh-101](https://github.com/bill9109/dsh-101) — DSH 文档阅读模式。
- [bill9109/dsh-drag-and-drop](https://github.com/bill9109/dsh-drag-and-drop) — 跨平台文件拖拽与原始路径插入，无需复制文件。
- [bobcat848/dsh-calculator](https://github.com/bobcat848/dsh-calculator) — 右侧面板展示 DeepSeek API 费用（当前会话 + 全部会话累计）与账户余额，内置官方计价与峰谷计价支持。
- [bpc-oss/dsh-web-billing](https://github.com/bpc-oss/dsh-web-billing) — 人民币/美元 token 计费，官方政策计价与逐条消息费用账本。
- [CanglongCl/dsh-web-review](https://github.com/CanglongCl/dsh-web-review) — 隔离网页预览，通过元素批注指导源码修改。
- [ccch1mneyyy/dsh-TUI](https://github.com/ccch1mneyyy/dsh-TUI) — Claude Code 风格全屏终端 UI：像素鲸鱼顶栏、实时工作状态行、思考流式展开。
- [ccq1/dsh-side-panel](https://github.com/ccq1/dsh-side-panel) — 侧边栏集成文件浏览器、终端和 Git 审查，方便预览文件。
- [daetz-coder/dsh-multi-chat](https://github.com/daetz-coder/dsh-multi-chat) — 在 DSH Web 界面里并排运行、监控多个对话实例的插件：多窗口墙 + 自动发现 + 单窗控制，内置带口令认证的局域网网关，手机/平板也能看。
- [dingyi222666/dsh-focus-chat](https://github.com/dingyi222666/dsh-focus-chat) — 「聚焦会话」精简视图，只关注最终产出结果。
- [dsh-paste-input](https://github.com/dsh-external/dsh-paste-input) — Ctrl+V 粘贴文件 / 拖拽 / 选择。
- [dsh-web-panel](https://github.com/dsh-external/dsh-web-panel) — 内嵌终端 dock + Git Review + 文件视图。
- [fishxcode/dsh-plugin-deepseek-balance](https://github.com/fishxcode/dsh-plugin-deepseek-balance) — 在 DSH Web 设置中展示 DeepSeek API 余额、余额趋势与每日用量图表。
- [Ghost011118/dsh-balance-meter](https://github.com/Ghost011118/dsh-balance-meter) — 输入框 dock 显示 DeepSeek 账户余额与会话花费，自动拉取官方定价，支持高峰/低谷计价。
- [GooodWei/context-vista](https://github.com/GooodWei/context-vista) — 右侧悬浮面板，环形图实时展示上下文 token 用量与费用。
- [Han-1413141/dsh-cost-meter](https://github.com/Han-1413141/dsh-cost-meter) — 会话与当日 API 费用统计、预算图框（已用%）、官方余额、历史看板，支持峰谷计价与官方价格一键同步。
- [Han-1413141/dsh-sticky-disclosure](https://github.com/Han-1413141/dsh-sticky-disclosure) — 一键收起会话中所有展开的区块（Think、工具卡等），常驻计数按钮 + 自定义快捷键。
- [huiliyi37/dsh-tianshu-tui](https://github.com/huiliyi37/dsh-tianshu-tui) — DeepSeek Harness 的终端 UI（TUI）。
- [jiangnanquan/dsh-ux](https://github.com/jiangnanquan/dsh-ux) — Solarized 浅色主题、紧凑布局、思考/工具链折叠胶囊，以及余额、本轮成本与用量看板的 DSH Web 界面增强插件。
- [Jolly-J/dsh-deepseek-billing](https://github.com/Jolly-J/dsh-deepseek-billing) — 侧边栏底部 DeepSeek 账户余额显示与会话费用估算卡片。
- [l541402398/dsh-file-uploads](https://github.com/l541402398/dsh-file-uploads) — 从 Web 输入框上传任意本地文件，以待发送卡片展示，并在设置中管理已存文件。
- [lak321/dsh-filetree](https://github.com/lak321/dsh-filetree) - 工程文件浏览器：会话视图文件页签，目录树 + VSCode 风格编辑器（C 语法高亮/行号/自动缩进/状态栏），跟随当前工作区。
- [lancecheney/dsh-deepseek-balance](https://github.com/lancecheney/dsh-plugins/tree/main/packages/dsh-deepseek-balance) — Session log 按钮左侧的实时计费徽章：余额、每会话消耗、峰谷/平价价格，按模型/货币/思考强度自动切换，每天抓官方定价。
- [Lanxing6480/dsh-galgame](https://github.com/Lanxing6480/dsh-galgame) — DSH Web 聊天界面 GalGame 演出层：立绘差分、流式思考气泡、打字机对话框与 GalGame 式提问/审批选项框，可随时切回普通聊天。
- [Laplace-bit/dsh-smooth-stream](https://github.com/Laplace-bit/dsh-smooth-stream) — 丝滑流式渲染：字跟着模型到达走、换行滑入、不闪，滚动归用户，尊重 `prefers-reduced-motion`。
- [lehhair/dsh-diff-viewer](https://github.com/lehhair/dsh-diff-viewer) — PiUI 风格 diff 查看器，替换 write/edit 工具调用的默认 DiffBlock。
- [lqhl/dsh-pi-tui](https://github.com/lqhl/dsh-pi-tui) — 差分渲染 TUI 前端：流式 Markdown 与工具卡片。
- [Luaphes/dsh-web-attention-badge](https://github.com/Luaphes/dsh-web-attention-badge) — 会话需要你时三处同时亮起：角标、标签页标题计数、按状态换色的鲸鱼 favicon。
- [Meredith2328/dsh-sticky-note](https://github.com/Meredith2328/dsh-sticky-note) — 编辑框工具栏便签，随手记点子和 TODO，自动保存为 Markdown，一键发送到对话。
- [MysaDC/dsh-plugin-description](https://github.com/MysaDC/dsh-plugin-description) — 为 Web 设置页插件卡片补上中英文功能说明。
- [Nagi-ovo/dsh-visualize](https://github.com/Nagi-ovo/dsh-visualize) — 对话内生成式 UI：模型把交互式 HTML 卡片直接画进会话流，带流式预览与沙箱渲染。
- [nonewind/dsh-spend](https://github.com/nonewind/dsh-spend) — DSH Web 用量与费用统计插件：右下角悬浮窗，按模型/按天/按会话多维聚合与预计花费。
- [omdsh-dev/dsh-annotation](https://github.com/omdsh-dev/dsh-annotation) — 选中文字→批注→随消息发送，回复按批注逐条对照。
- [omdsh-dev/dsh-at-file](https://github.com/omdsh-dev/dsh-at-file) — Codex 风格的 `@file` 文件引用，输入框里直接搜索并引用工作区文件。
- [omdsh-dev/DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) — 侧边栏完整工作台：内置文件渲染编辑、终端、Git 与子代理，支持三方插件注册新 Tab。
- [omdsh-dev/dsh-genui](https://github.com/omdsh-dev/dsh-genui) — 助手回复内渲染交互式 UI 组件：布局、图表、表单、测验、mermaid、3D 场景与回传事件循环。
- [omdsh-dev/ex-setting](https://github.com/omdsh-dev/ex-setting) — DSH 的设置扩展。
- [omdsh-dev/web-components](https://github.com/omdsh-dev/web-components) — Web Components 支持。
- [openma-ai/deepseek-harness-tui](https://github.com/openma-ai/deepseek-harness-tui) — Rust/ratatui 终端客户端，直接使用 DSH SDK JSON-RPC 协议，支持独立运行或作为 profile bundle 加载。
- [pk7j7sqryy-ops/dsh-token-pet](https://github.com/pk7j7sqryy-ops/dsh-token-pet) — 会话头部卡通用量小部件：布布玩偶 + 上下文占用/会话累计/构成，附日期周几、天气、3 天预报与极端天气预警（雨滴/雪花动画），跟随主题色。
- [qyw233/dsh-deeplink](https://github.com/qyw233/dsh-deeplink) — `?session=` / `?workspace=` 深链直达指定项目对话。
- [renat3u/dsh-web-archive](https://github.com/renat3u/dsh-web-archive) — 折叠对话中的 Think、Bash 等「无用消息」。
- [Sev7een/ds-api-usage](https://github.com/Sev7een/ds-api-usage) — 在设置页展示 DeepSeek API 余额与最近 24 小时用量，包括估算消费、Token、请求次数和按小时时间线。
- [Simon314620/dsh-turn-index](https://github.com/Simon314620/dsh-turn-index) — 轮次索引侧边栏，滚动时自动高亮当前轮次。
- [SnowCrescenter-tech/dsh-milestone](https://github.com/SnowCrescenter-tech/dsh-milestone) — 右侧圆点时间轴导航条，点击跳转到任意用户消息。
- [Starfie1d1272/dsh-builtin-toggles](https://github.com/Starfie1d1272/dsh-builtin-toggles) — 为 DSH Web 添加官方内置插件目录、搜索与状态说明，并提供经过审核的安全 UI 插件开关。
- [stopchewing/dsh-mcp-view](https://github.com/stopchewing/dsh-mcp-view) — MCP 服务器与工具清单面板：侧边栏一键悬浮面板，按服务器分组展示全部 MCP 工具（传输方式、端点、JSON Schema、最近使用时间），默认折叠、支持搜索与实时刷新；最近使用时间来自真实会话日志。
- [Sttrevens/dsh-cost-meter](https://github.com/Sttrevens/dsh-cost-meter) — Web UI 美元成本徽标：头部显示会话总成本、每条回复结尾显示该轮成本，悬停看分项。
- [v587d/dsh-opencode-go-usage](https://github.com/v587d/dsh-opencode-go-usage) — 在输入框上方 dock 显示 OpenCode Go 订阅用量（5h 滚动/每周/每月窗口与重置倒计时），内置凭据编辑器。
- [vibeinging/dsh-turn-navigator](https://github.com/vibeinging/dsh-turn-navigator) — 对话轮次导航。
- [vlln/dsh-navbar](https://github.com/vlln/dsh-navbar) — 对话节点导航条，右缘节点串快速跳转 user 消息。
- [vlln/dsh-task-status](https://github.com/vlln/dsh-task-status) — 后台任务状态条：对话页任务进度 + 实时输出 tail。
- [WFMinerva/dsh-turn-cost](https://github.com/WFMinerva/dsh-turn-cost) — 每条 AI 回复下方显示该轮真实花费：人民币、官方峰谷价、缓存读占比；纯本地读会话日志，零上报零密钥。
- [wsxwj123/dsh-plugins#turn-scrubber](https://github.com/wsxwj123/dsh-plugins/tree/main/packages/turn-scrubber) — 右侧紧凑回合刻度条，悬停显示回合摘要，点击跳转到对应用户回合。
- [xiaogu619520/dsh-plugin-task-panel](https://github.com/xiaogu619520/dsh-plugin-task-panel) — 任务摘要与上下文用量监控浮动面板（待办事项跟踪、文件与系统 Token 占用统计、8向缩放与快捷键）。
- [yoli-mi/dsh-client-ui-custom](https://github.com/yoli-mi/dsh-client-ui-custom) — Web 外观主题定制（壁纸、毛玻璃、强调色、预设）、键盘快捷键、用量统计、插件市场、浮动历史条与用户消息 Markdown 渲染。
- [yyyyukari/dsh-plugin-workshop](https://github.com/yyyyukari/dsh-plugin-workshop) — 创意工坊式插件浏览器：一键安装/更新/卸载。
- [zealot00/dsh-pet](https://github.com/zealot00/dsh-pet) — DSH Web UI 桌面宠物：精灵图动画、agent 状态联动、拖拽、闹钟（每天/一次）与番茄钟，皮肤下拉选择 + 预览。
- [zh667/TokenLedger](https://github.com/zh667/TokenLedger) — 按中转站点、项目和模型统计本地 DSH Token 用量，并显示账户余额与订阅额度周期。
- [Zhangbo-cn/dsh-voice-input-plugin](https://github.com/Zhangbo-cn/dsh-voice-input-plugin) — 输入框麦克风：点击持续监控、按住对话；浏览器语音识别逐字上屏，回复由 host Edge TTS 边生成边朗读（句子切分），朗读时暂停识别防回声，点击可停止。
- [zhu1090093659/dsh-web-ui](https://github.com/zhu1090093659/dsh-web-ui) — DSH Web UI 插件与皮肤合集：任务看板、git 图、右侧面板、远程移动端 UI、桌宠、实时 token 统计与皮肤中心。
- [ZSeven-W/dsh-openpencil](https://github.com/ZSeven-W/dsh-openpencil) — OpenPencil 设计预览与编辑插件。

### 🎭 主题与外观
- [BeiZi6/dsh-theme-plugin](https://github.com/BeiZi6/dsh-theme-plugin) — DSH Web GUI 主题工作室：5 套内置预设 + 完全可自定义的浅/深配色（强调色、背景、前景、UI 与代码字体、半透明侧栏、对比度），即时热切换并持久化到 localStorage。
- [Braidy-Wu/dsh-conversation-minimap](https://github.com/Braidy-Wu/dsh-conversation-minimap) — DSH Web GUI 对话迷你地图（复刻 ChatGPT 桌面端）：每轮 Prompt 一个等距胶囊锚点，鱼眼钟形悬停放大 + 完整 Prompt 预览，顶部/底部渐隐，蓝色高亮跟随当前 Prompt，点击跳转对应消息，自动拉取完整历史。
- [dsh-skins](https://github.com/dsh-external/dsh-skins) — Web UI 皮肤。
- [ink5897/dsh-theme-kit](https://github.com/ink5897/dsh-theme-kit) — 32 款预设主题（莫兰迪 / 马卡龙 / 中国传统色）、动态与静态壁纸、纸纹纹理、分区透明度与文字深浅，附按键桌宠。
- [dsh-custom-theme-import](https://github.com/Juryorca/dsh-custom-theme-import) — DSH Web 自定义主题导入插件：支持本地路径/GitHub 集合一键导入、主题预览与实时刷新、托管主题库；格式轻量，作者可直接改 CSS/DOM 文件热加载，适合个人主题开发与分享。
- [KinGao294/dsh-skin](https://github.com/KinGao294/dsh-skin) — Codex 风格皮肤切换器 + 自定义壁纸层，可调透明度与模糊。
- [Liu-ZA-81/dsh-theme-firefly](https://github.com/Liu-ZA-81/dsh-theme-firefly) — 崩坏：星穹铁道「流萤」主题：立绘/动态壁纸、萤火绿霓虹配色、开屏变身动画、萤火氛围粒子、背景音乐、打字音效与按对话触发的表情包彩蛋。
- [dsh-odette-skin](https://github.com/lkdx0220/Genshin-odette-skin-dsh) — DSH 原神「奥黛塔」主题 UI 皮肤：深/浅双模式背景图 + 13 个主题 token 毛玻璃覆盖 + 侧栏 Q 版小兽皮肤开关，npm 即装即用。
- [RevolutionLA/dsh-dream-skin](https://github.com/RevolutionLA/dsh-dream-skin) — DSH Web 一键换肤插件：8 套原创主题、背景壁纸（透明度/模糊/渐变/URL）、每用户强调色、主题包导入导出与分享链接、收藏与随机，纯原生 token 系统。
- [Small-tailqwq/dsh-deep-whale](https://github.com/Small-tailqwq/dsh-deep-whale) — DSH Web 鲸鱼娘皮肤系列（深海女仆工坊 maid-atelier）。
- [wsxwj123/dsh-plugins#theme-gallery](https://github.com/wsxwj123/dsh-plugins/tree/main/packages/theme-gallery) — 15 个精选主题家族，浅深配色完整，跟随 DSH 原生浅色/深色/跟随系统模式。
- [xiaoyanzi191/dsh-premium-themes](https://github.com/xiaoyanzi191/dsh-premium-themes) — 8 套精选配色方案与自定义调色板导入（名称+方案+种子色推导完整 token 映射），设置页「调色板」行，热插拔安装。
- [zhtx2024/dsh-skin-switcher](https://github.com/zhtx2024/dsh-skin-switcher) — 在设置界面新增「皮肤」页，自动发现已安装皮肤并一键切换，支持一键恢复官方默认外观。

### 💬 会话与消息
- [Anionex/dsh-turn-rewind](https://github.com/Anionex/dsh-turn-rewind) — 对话回退：基于持久 Change Ledger 回滚会话与工作区状态。
- [bill9109/dsh-conversation-share](https://github.com/bill9109/dsh-conversation-share) — 分享任意段落的对话。
- [Buyi-wsgzg/dsh-sidechain](https://github.com/Buyi-wsgzg/dsh-sidechain) — `/side` 持续性侧会话与 `/btw` 一次性侧问，在临时 fork 中运行、不写入主会话历史。
- [chenproton/dsh-history](https://github.com/chenproton/dsh-history) — 会话历史消息查看：列出当前会话全部你发送的消息，支持排序、搜索、一键复制与点击跳转定位（目标未加载时自动加载更早历史）。
- [Chinesezjc/dsh-interconnect](https://github.com/Chinesezjc/dsh-interconnect) — 跨实例互联：经 interconnect 服务在多个 DSH 实例间转发消息与事件。
- [czm15053/dsh-peer-link](https://github.com/czm15053/dsh-peer-link) — 让 dsh 和 Claude Code 会话直接互发消息，附带可点击的会话列表卡片（搜索/刷新/弹窗发送）。
- [dsh-session-search](https://github.com/dsh-external/dsh-session-search) — 跨 dsh/Codex/Claude Code/pi/OpenCode 会话只读搜索，无索引。
- [edfrey0044/dsh-unarchive](https://github.com/edfrey0044/dsh-unarchive) — 恢复已归档会话：/unarchive 命令与 unarchive_session 工具，把会话移出归档集合、在原位置重新出现在工作区（归档从不删除数据）。
- [flyingtimes/dsh-trajectory-reader](https://github.com/flyingtimes/dsh-trajectory-reader) — 轨迹解读标签页：按用户轮次解读助手做了什么（需求/思路/执行/结果），规则引擎 + 可选 LLM 叙述，文件/命令/错误一目了然，用户消息原样保留。
- [futongxu9-maker/dsh-msgrail](https://github.com/futongxu9-maker/dsh-msgrail) — 对话右缘消息轨道：每条用户消息一个品牌色圆点，悬停预览、点击跳转、自动加载未加载历史，纯插件零宿主侵入。
- [hellodigua/dsh-share](https://github.com/hellodigua/dsh-share) — 一键分享你的对话。
- [Jesse-njx/dsh-crosstalk](https://github.com/Jesse-njx/dsh-crosstalk) — 跨会话消息：本机任意会话都可像 Claude Code 一样列出并互发消息，基于本地心跳注册表与收件箱。
- [session-titler](https://github.com/JohnXu22786/session-titler) — 双阶段会话标题生成：忙碌时即时关键词标题，空闲时由经济模型精修。
- [Moeblack/dsh-message-edit](https://github.com/Moeblack/dsh-message-edit) — 基于分支的消息编辑、reroll、重试与版本时间线。
- [Moeblack/dsh-prompt-studio](https://github.com/Moeblack/dsh-prompt-studio) — 带实时预览的用户/内置 system prompt 分节编辑器。
- [Nwflower/dsh-chat-import](https://github.com/Nwflower/dsh-chat-import) — 把 Claude Code / Codex / ChatGPT / Cursor / Gemini / Reasonix / opencode 的聊天记录全保真导入为可续聊的 DSH 会话。
- [Nwflower/dsh-file-claim](https://github.com/Nwflower/dsh-file-claim) — 同一工作区并行多会话的文件认领与写入保护（claim/release、心跳 stale 接管、pending 三路合并）。
- [sjh9714/dsh-what-changed](https://github.com/sjh9714/dsh-what-changed) — 整会话改动审阅。会话顶栏列出本次 Agent 写过的每个文件与逐处改动，被权限拒绝的写入单独计数不算改动，数据来自 session projection。
- [Wine-Red/dsh-prompt-stash](https://github.com/Wine-Red/dsh-prompt-stash) — 本地、按会话隔离的 LIFO 输入暂存：临时收起未完成的输入，之后安全恢复并继续编辑。
- [yuezengwu/dsh-explain](https://github.com/yuezengwu/dsh-explain) — 本地优先学习模式：跨会话全局学习线程、按来源讲解。

### 🧠 记忆
- [bowenliang123/dsh-context](https://github.com/bowenliang123/dsh-context) — 上下文洞察面板：一眼看清模型上下文窗口的组成与变化——构成对照窗口大小、按请求历史趋势、压缩/注入事件、消息级 token 统计。
- [Breeze136/dsh-kb-rag](https://github.com/Breeze136/dsh-kb-rag) — 本地文献知识库 RAG：8 个工具（PDF/文件夹/Zotero 入库、BM25+向量+重排混合检索、DOI 可点击溯源问答、范围/严格模式、去重/清空/统计），全本地 bge 嵌入 + 单文件 SQLite，实测 242 篇 86s 入库、2 万块亚秒热查询。
- [flymysql/dsh-memory](https://github.com/flymysql/dsh-memory) — 跨会话记忆库：remember / recall / forget 工具、每轮提示注入与设置页条目浏览。
- [freehul/sgme](https://github.com/freehul/sgme) — 拾光记忆引擎（SGME）桥接：多智能体共享长期记忆（HTTP）—— L0/L1/L1.5/L2 分层提炼、按场景注入、统一检索、主动关怀信号（memory_search / wiki_search / signal_pull / signal_claim / signal_ack），npm 包名 `dsh-sgme`。
- [futongxu9-maker/dsh-shared-memory](https://github.com/futongxu9-maker/dsh-shared-memory) — 跨对话共享记忆：MEMORY.md + USER.md 注入每个会话系统提示词，memory 工具 + 可视化记忆面板，Hermes 式实现。
- [ICCuse/dsh-file-memory](https://github.com/ICCuse/dsh-file-memory) — 文件型工作记忆：memorize/recall 把关键前提逐字保存在会话笔记文件，无损挺过上下文压缩。
- [ICCuse/dsh-knowledge](https://github.com/ICCuse/dsh-knowledge) — 全局 Markdown 知识库桥：kb_add/kb_search/kb_show/kb_timeline 读写与 Codex kb.cmd CLI 共享的知识库（格式逐字节兼容）。
- [ICCuse/dsh-premise-guard](https://github.com/ICCuse/dsh-premise-guard) — 压缩后前提漂移守卫：摘要丢失关键字面锚点时注入一次性提醒。
- [Jesse-njx/dsh-memory](https://github.com/Jesse-njx/dsh-memory) — 基于 DSH 无损会话日志的引用式记忆：蒸馏出的事实带 `(sessionId, eventRange)` 引用，可随时展开回原始日志片段。
- [memory-vault](https://github.com/JohnXu22786/memory-vault) — 跨会话持久记忆插件：SQLite 本地存储 + 关键词/语义混合检索 + Web/MCP 界面，供编码代理存取经验与决策。
- [LoserFox/distill](https://github.com/LoserFox/distill) — 自动对话蒸馏：后台 subagent 反省 + 技能 create/update。
- [modusensus/dsh-mneme](https://github.com/modusensus/dsh-mneme) — 跨会话记忆：SQLite + 可人工编辑的 Markdown 镜像，后台自动巩固（去重/合并/冲突裁决），提供 6 个记忆工具。
- [nowledge-co/nowledge-mem-deepseek-harness](https://github.com/nowledge-co/nowledge-mem-deepseek-harness) — 给所有 AI 工具和 Agent 共用的一层记忆：注入 Context Bundle、提示时检索、MCP 工具与回合结束 DSH 线程捕获。
- [omdsh-dev/dsh-mnemon](https://github.com/omdsh-dev/dsh-mnemon) — Mnemon 深度集成：本地三层记忆（Runtime Memory、可检索 Documents、受监督 Memory Spaces）。
- [PerryLink/dsh-memento](https://github.com/PerryLink/dsh-memento) — 有界、分层、带审批门、可审计的跨会话记忆：`ctx.memory` 服务 + 零依赖 SQLite 存储 + `memory` 工具与冻结快照注入；写入必过审批门，模型可见内容可自会话日志重建。
- [Phant0Meow/dsh-memory-meow](https://github.com/Phant0Meow/dsh-memory-meow) — 项目级跨会话记忆：PROJECT.md 快照注入首条用户消息（缓存友好）+ memory_remember 工具 + ReAct 任务结束自动反思；各项目独立记忆文件，互不互通。
- [Tyan66666/billion-context-dsh](https://github.com/Tyan66666/billion-context-dsh) — 模型驱动的上下文压缩：由模型决定何时压缩、压缩什么。
- [xiejianjun000/eco-dsh-plugins](https://github.com/xiejianjun000/eco-dsh-plugins) — 评分制记忆树插件 eco-memory-tree：结构化长期记忆，BM25/中文检索，Obsidian 双向同步。
- [Xplore-LAB/dsh-plugin-asmemory](https://github.com/Xplore-LAB/dsh-plugin-asmemory) — 动作-状态时序记忆：记录类型化的状态与动作，做趋势、异常与因果关联分析。

### 🛠️ 工具与能力
- [1na-ko/dsh-hdc-bridge](https://github.com/1na-ko/dsh-hdc-bridge) — 鸿蒙设备桥：hdc 截图/装包/日志/崩溃/UI 自动化闭环（配 read_image 看图），官方优先版本化 API 知识层（SDK .d.ts + 离线随包文档），以及 DevEco CLI 构建/签名/lint 通道。
- [dsh-verify](https://github.com/263311487-ux/dsh-verify) — 独立浏览器验收测试：JSON 清单驱动真实 Chromium，断言计算样式与像素差异，输出 HTML 报告 + 0/1 退出码；提供 npm CLI、GitHub Action 与 MCP Server。
- [acefun29/dsh-file-mount](https://github.com/acefun29/dsh-file-mount) — 文件增量挂载与重复读取去重：已挂载行范围不重复进上下文。
- [AlloyPlane/dsh-eye-vision](https://github.com/AlloyPlane/dsh-eye-vision) — 纯文本模型识图桥接：通过任意 OpenAI 兼容多模态 API 提供 image_understand 工具（识图/OCR/UI 分析），支持允许目录白名单。
- [Anionex/dsh-computer-use](https://github.com/Anionex/dsh-computer-use) — macOS 电脑控制：Accessibility 观测、过期状态拒绝、作用域权限与安全输入。
- [Anionex/dsh-vision-toolkit](https://github.com/Anionex/dsh-vision-toolkit) — 让纯文本模型更好地做视觉任务：带意图的图片问答、长截图 OCR、UI 还原等。
- [Anlushu/hkinsure](https://github.com/Anlushu/hkinsure) — 香港保险数据 MCP：260+ 真实产品、17 家保司、分红实现率，供 Hermes / dsh / Claude Code 等 AI 工具查询/对比/测算。
- [awesome-dsh-plugin/dsh-find-plugin](https://github.com/awesome-dsh-plugin/dsh-find-plugin) — 会话内直接找插件：按关键词/分类搜索本精选 registry，返回描述与可直接执行的安装命令。
- [beancookie/dsh-plugin-anydoc](https://github.com/beancookie/dsh-plugin-anydoc) — 将 @firecrawl/anydoc 作为 anydoc 工具注册给 Agent，把 Word/PPT/Excel/PDF/EPUB 等多种文档格式转换为 GitHub-Flavored Markdown。
- [canghai666x/dsh-news-plugin](https://github.com/canghai666x/dsh-news-plugin) — RSS 新闻采集工具，抓取 10+ 中英文源为结构化条目。
- [cdxiaodong/dsh-llm-inspector](https://github.com/cdxiaodong/dsh-llm-inspector) — 统一 LLM 请求/响应检查器：调 reasoning effort、外部思考(think)导出、流量与包分析。
- [cendaifeng/dsh-learn-everything](https://github.com/cendaifeng/dsh-learn-everything) — 费曼学习法教学闭环，渲染为富 HTML 教学卡片。
- [chushixixin/dsh-harness-mcp-server](https://github.com/chushixixin/dsh-harness-mcp-server) — MCP server 让任意 MCP 客户端驱动 Harness agent。
- [ciceroyang/dsh-report-studio](https://github.com/ciceroyang/dsh-report-studio) — 把 DSH 会话一键变成日报/周报/交接文档/文章，附可验证凭据。
- [browser4-dsh](https://github.com/dsh-external/browser4-dsh) — Browser4 AI-native 浏览器引擎（skills）。
- [dsh-browser-panel](https://github.com/dsh-external/dsh-browser-panel) — WebUI 内嵌有头浏览器，模型实时操控、0 视觉依赖。
- [dsh-office](https://github.com/dsh-external/dsh-office) — 模型读写 Office 文件，web 客户端 docx/pdf 预览。
- [dsh-market/dsh-market](https://github.com/dsh-market/dsh-market) — 装在 DSH 里的插件市场：设置页内逛/搜全部社区插件，按分类筛选，确认后一键安装，已装插件一目了然。
- [EvilIrving/dsh-context-proxy](https://github.com/EvilIrving/dsh-context-proxy) — 按需取回薄层：context_query / context_slice / context_grep 三个工具读取已持久化的历史，引用可回放。
- [flymysql/dsh-remote](https://github.com/flymysql/dsh-remote) — 远程工作区：SSH 密码或 key 连接远程主机，选取远程工作区目录，用 rw_pick_workspace / rw_list_dir / rw_read_file / rw_exec 工具在远程直接操作。
- [futongxu9-maker/dsh-path-reveal](https://github.com/futongxu9-maker/dsh-path-reveal) — 点击消息里的 Windows 绝对路径在资源管理器中打开所在文件夹（文件定位选中/目录直接打开）。
- [gloryxpnv/dsh-tool-vision](https://github.com/gloryxpnv/dsh-tool-vision) — 为纯文本 DeepSeek Harness 提供本地优先视觉：由本地 VLM（LM Studio / Ollama / vLLM）产出结构化 JSON 证据（OCR / 版面 / 语义），零 API 成本，图片数据完全不出本机。
- [gongyijie85/dsh-repo-setup](https://github.com/gongyijie85/dsh-repo-setup) — 只读仓库体检引导工具（repo_setup_scan）：识别技术栈/测试/文档/git/数据库线索，给出技能插件、MCP 服务器与卫生文件的安装建议（claude-code-setup 的 DSH 对应）。
- [Gumiho12345/dsh-plugin-net-access](https://github.com/Gumiho12345/dsh-plugin-net-access) — DSH 的 net-access 权限模式：文件写保护不变，沙箱内 curl.exe 可用 HTTPS（Windows）。
- [hccccc01333/dsh-excel-chat](https://github.com/hccccc01333/dsh-excel-chat) — 在 DeepSeek Harness 里对话完成 Excel 工作：建表、编辑、修复公式、图表校验，每次编辑后自动体检公式。
- [HuanLinOTO/dsh-plugin-mineru](https://github.com/HuanLinOTO/dsh-plugin-mineru) — 向模型暴露 MineRU 文档解析工具。
- [huey1in/trio](https://github.com/huey1in/trio) — 浏览器自动化（Playwright，带实时画面）+ MCP Server（把 DSH agent 暴露给任何 MCP 客户端）+ GitHub issue/PR/webhook 评审工具。
- [IWAIBAOLI/dsh-with-pencil](https://github.com/IWAIBAOLI/dsh-with-pencil) — 将官方 pen.dev Pencil 设计能力接入 DeepSeek Harness：桥接官方 CLI，Agent 可在会话中编辑 .pen 文件，并针对 DeepSeek 纯文本模型做了专门优化。
- [Jesse-njx/dsh-cowork](https://github.com/Jesse-njx/dsh-cowork) — doc_read/doc_write：以有界、单元格寻址的方式读写 xlsx / pdf / docx / pptx / ipynb，另附 MCP 服务器与 CLI。
- [Jesse-njx/dsh-docker](https://github.com/Jesse-njx/dsh-docker) — 类型安全、带护栏的容器控制：ps/logs/inspect/exec/start/stop 与 compose up/down，JSON 输出、项目感知定位、破坏性操作需审批。
- [Jesse-njx/dsh-skillport](https://github.com/Jesse-njx/dsh-skillport) — 把已有的 Agent Skills（SKILL.md）技能库带进 DSH：扫描 Claude/Codex/Cursor/Gemini 技能目录、注入渐进式索引，按需加载技能正文。
- [Jesse-njx/dsh-voice](https://github.com/Jesse-njx/dsh-voice) — 语音输入、语音输出：把口述音频转写为用户消息（transcribe），让 agent 朗读回复（speak），本地优先，音频存于 ~/.dsh/voice。
- [jihongboo/dsh-apple-mode](https://github.com/jihongboo/dsh-apple-mode) — DSH 的 Xcode AI 集成：26 个 Xcode MCP 工具（mcpbridge）+ Apple 平台技能 + Xcode Intelligence 风格 persona（agent preset 或全局 bundle）。
- [adversarial-review](https://github.com/JohnXu22786/adversarial-review) — gavel-review：对抗式多视角代码审查——并行攻击视角、确定性静态哨兵、严重度定级与审查历史。
- [browser-automation](https://github.com/JohnXu22786/browser-automation) — Web Bridge：面向 dsh 的浏览器自动化 MCP 服务器——真实浏览器导航、点击、填表、截图、JS 执行，无障碍快照驱动。
- [codegraph](https://github.com/JohnXu22786/codegraph) — 代码知识图谱：把符号、调用点与导入索引进 SQLite，回答调用/依赖问题。
- [command-scout](https://github.com/JohnXu22786/command-scout) — 扫描项目声明的构建命令（Makefile、package.json scripts、justfile、deno tasks）并作为 agent 工具暴露。
- [computer-control](https://github.com/JohnXu22786/computer-control) — 桌面控制：屏幕捕获、指针/键盘注入、无障碍树操作、确认流程与紧急停止。
- [context-pruner](https://github.com/JohnXu22786/context-pruner) — 会话上下文整理插件：修剪过期、重复、失败与过大的上下文以节省 token 预算。
- [docs-retriever](https://github.com/JohnXu22786/docs-retriever) — doctrove：版本化库文档检索 MCP 服务器，零运行时依赖，可作 dsh 插件 bundle 安装。
- [fs-mcp](https://github.com/JohnXu22786/fs-mcp) — paddock：受限本地文件系统 MCP 服务器——文件访问限定在可配置区域，零运行时依赖。
- [github-mcp](https://github.com/JohnXu22786/github-mcp) — repogate：GitHub 开发者工作台 MCP 服务器——仓库、issue、PR、代码审查、搜索，零运行时依赖。
- [pty-runner](https://github.com/JohnXu22786/pty-runner) — 后台终端（PTY）任务管理：启动长时进程、喂入输入、翻页输出、按需停止。
- [safety-net](https://github.com/JohnXu22786/safety-net) — 编码 agent 破坏性命令拦截闸门：rm -rf / git reset --hard / push --force 执行前解析判定并要求人工确认（dsh 插件 + 通用 CLI）。
- [secret-guard](https://github.com/JohnXu22786/secret-guard) — 阻止 agent 读写敏感文件（.env、凭据），掩码工具结果中泄露的密钥，附审计日志与安全的 sg_* 检查工具。
- [snippet-expander](https://github.com/JohnXu22786/snippet-expander) — Steno：发送前的行内 #tag 快捷展开——多库、别名、{{变量}}、递归防护。
- [statusline](https://github.com/JohnXu22786/statusline) — 实时终端状态行：一行展示模型、上下文占用、子代理、速率限制与会话时长。
- [worktree-mgr](https://github.com/JohnXu22786/worktree-mgr) — 任务隔离的 git 工作区：按任务自动创建、同步与收尾隔离工作区。
- [kunjinkao-os/dsh-mobile-gui-agent](https://github.com/kunjinkao-os/dsh-mobile-gui-agent) — Android GUI Agent：ADB 截图、压缩 UI hierarchy 定位、逐步动作验证、审批和 Mobile Web 视图。
- [lak321/dsh-screen-agent](https://github.com/lak321/dsh-screen-agent) — 桌面与网页自动化：📸 多屏截图 + 🔍 Windows OCR（文字+像素坐标）+ 🖱️ 鼠标点击/拖拽 + ⌨️ 中文打字/按键 + 🪟 窗口激活，含实战打磨的画图能力（鼠标加速度补偿、画布定位、贝塞尔曲线，可在画图中绘制图形）。
- [lak321/dsh-voice-chat](https://github.com/lak321/dsh-voice-chat) — 语音对话：🎤 语音输入（Web Speech，实时中间结果可编辑）+ 🔊 自动/手动朗读回复（TTS），支持人声/语速/语调设置与识别语言（普通话/粤语等），纯客户端零密钥，朗读前自动清理 Markdown 标记。
- [Letter2025/dsh-task-worktree](https://github.com/Letter2025/dsh-task-worktree) — 完整的任务级 git worktree：per-repo manifest 永久保存、worktree-<name> 分支、主目录带回（bring-back）与直接提交两种收尾、可携带主工作区未提交改动（参考 Qoder / Codex / Claude Code）。
- [lire1131/dsh-undo-plugin](https://github.com/lire1131/dsh-undo-plugin) — DSH 撤销/回退系统：配置变更自动存档，一键撤销/恢复/回退到任意版本，支持 WebUI 与离线 CLI/GUI 工具（DSH 启动失败也能救）。
- [liustack/modlens](https://github.com/liustack/modlens) — 为纯文本模型架起视觉桥梁：粘贴图片，输出结构化 JSON 证据（OCR、版面、语义）。
- [liustack/modsearch](https://github.com/liustack/modsearch) — 纯文本 agent 的联网搜索桥：搜索网页与 X，返回结构化 JSON 证据（search/fetch/引用）。
- [lonelymoon87/dsh-code-intel](https://github.com/lonelymoon87/dsh-code-intel) — 用 Tree-sitter 建立工作区符号索引，提供词法或可选 embedding 辅助的代码检索。
- [lsjspl/dsh-plugin-grok2api-media-tool](https://github.com/lsjspl/dsh-plugin-grok2api-media-tool) — 让 dsh 通过 grok2api 的 API 获得生成图片与视频能力。
- [Luke-Yong/dsh-plugin-knowledge-graph](https://github.com/Luke-Yong/dsh-plugin-knowledge-graph) — 基于代码库知识图谱的 read_graph 工具（CONTAINS / EXPORTS / IMPORTS / IMPORTS_SYMBOL 关系）。
- [Lum1104/dsh-browser](https://github.com/Lum1104/dsh-browser) — Chrome 侧边栏扩展，让 DSH 直接操控你的浏览器，无需视觉能力。
- [lxj808624/dsh-tool-git](https://github.com/lxj808624/dsh-tool-git) — 结构化 Git 工具（status/diff/log/branch/stage/commit）+ 破坏性命令安全护栏。
- [lynx-gt/dsh-subagent-cwd](https://github.com/lynx-gt/dsh-subagent-cwd) — 在 dsh-subagent-tools 基础上增加子代理按调用 cwd，附带所需的两个 in-process provider 补丁。
- [lynx-gt/dsh-subagent-tools](https://github.com/lynx-gt/dsh-subagent-tools) — 子代理委派的按调用覆盖：model/provider/persona/toolFilter、@preset: 引用与 provider/model 组合 id。
- [lzszq/dsh-scholar](https://github.com/lzszq/dsh-scholar) — 学术助手插件。
- [maddogfinance/dsh-trading](https://github.com/maddogfinance/dsh-trading) — 只读交易研究工作台：类型化行情数据接缝（可自带数据源）、多周期指标 regime 快照、dsh web 交互式 K 线卡（AI 标注需引用依据并经真实 K 线区间校验）、结构性禁止下单的 risk-guard。
- [MAXeaglet/dsh-bash-terminal](https://github.com/MAXeaglet/dsh-bash-terminal) — 一个 shell 工具：Windows 上统一执行 PowerShell / Git Bash / WSL，外加交互式 PTY 终端，默认终端由用户在设置中选择。
- [moon09300731/dsh-approval-gate](https://github.com/moon09300731/dsh-approval-gate) — 自动审批门控：Flash 预判写入/命令是否不可回补，安全操作自动批准、危险操作转人工（fail-safe）。
- [moon09300731/dsh-vision-tools](https://github.com/moon09300731/dsh-vision-tools) — DeepSeek Harness 视觉能力全家桶：vision_understand 工具（OpenAI 兼容视觉 API，默认免费智谱 GLM-4V-Flash）+ 粘贴/拖拽/按钮三入口识图。
- [omdsh-dev/dsh-custom-tool](https://github.com/omdsh-dev/dsh-custom-tool) — 用 Monaco 编辑器创建和管理沙箱化的自定义 JavaScript 工具。
- [omdsh-dev/dsh-data-agent](https://github.com/omdsh-dev/dsh-data-agent) — 让 AI 帮你连数据库、写 SQL。
- [omdsh-dev/dsh-kb-sieve](https://github.com/omdsh-dev/dsh-kb-sieve) — 从 md/txt/docx/pdf 构建可审计知识库包（SQLite FTS5），确定性检索与原文阅读。
- [omdsh-dev/dsh-tool-calculator](https://github.com/omdsh-dev/dsh-tool-calculator) — 安全的数学表达式求值器，零依赖递归下降解析器。
- [omdsh-dev/dsh-tool-csv](https://github.com/omdsh-dev/dsh-tool-csv) — CSV 解析/查询/统计/转换（RFC 4180），零依赖状态机解析器。
- [omdsh-dev/dsh-tool-diff](https://github.com/omdsh-dev/dsh-tool-diff) — 文本/JSON/CSV/Markdown 结构化比较与 unified diff。
- [omdsh-dev/dsh-tool-encoding](https://github.com/omdsh-dev/dsh-tool-encoding) — base64/url/hex 编解码、常用哈希、UUID 生成。
- [omdsh-dev/dsh-tool-json](https://github.com/omdsh-dev/dsh-tool-json) — JMESPath 子集 JSON 查询。
- [omdsh-dev/dsh-tool-markdown](https://github.com/omdsh-dev/dsh-tool-markdown) — HTML↔Markdown 转换、GFM 表格规范化、目录生成。
- [omdsh-dev/dsh-tool-regex](https://github.com/omdsh-dev/dsh-tool-regex) — 正则测试/提取/安全替换/静态解释（不执行代码）。
- [omdsh-dev/dsh-tool-schema](https://github.com/omdsh-dev/dsh-tool-schema) — JSON Schema 验证：validate/paths/explain/normalize。
- [omdsh-dev/dsh-tool-stat](https://github.com/omdsh-dev/dsh-tool-stat) — 描述统计/百分位数/频数分布/相关性。
- [omdsh-dev/dsh-tool-time](https://github.com/omdsh-dev/dsh-tool-time) — 严格 ISO 8601 解析、IANA 时区转换、UTC 日历运算。
- [omdsh-dev/dsh-toolkit](https://github.com/omdsh-dev/dsh-toolkit) — 零依赖工具包：time / encoding / json / calculator / csv / regex / markdown / diff / stat / schema 十件套一键安装。
- [phelpsyacht/dshmath-manim](https://github.com/phelpsyacht/dshmath-manim) — 基于 Manim CE 的数学动画插件：6 个内置模板（函数/导数/积分/几何/极坐标/3D 曲面）+ 零代码技能包（math-animation / manim-codegen），模型说人话即可生成动画视频，含 AST 静态安全校验。
- [PicGo/dsh-plugin](https://github.com/PicGo/dsh-plugin) — 通过 PicGo 已有配置（PicGo Cloud、GitHub、S3、腾讯云 COS、七牛，或任意已安装的上传插件）把本地图片和文件上传到图床，提供 `picgo_upload` 工具与 `/picgo` 命令。
- [PolinniZhong/dsh-omi-voice](https://github.com/PolinniZhong/dsh-omi-voice) — 豆包音质对话内朗读：每条 AI 回复 🔊 点读/自动朗读（默认关、状态持久化），音色由本地 Omi 引擎合成（豆包 seed-tts），BYOK（Key 只留在本机 Keychain，插件零 Key）。
- [sakikoTGW/pack-agent](https://github.com/sakikoTGW/pack-agent) — 把 .pack.json/.pack.zip 投影到 .agent-pack/modpacks/，按工作区白名单暴露 skill。
- [SamXiaBing/dsh-adb](https://github.com/SamXiaBing/dsh-adb) — ADB 设备·台架运维工具集：设备发现、结构化 logcat（后台采集）、apk 安装、文件 pull/push、性能快照。
- [Sanqi-normal/dsh-webui-market-plugin](https://github.com/Sanqi-normal/dsh-webui-market-plugin) — dsh Web GUI 内的社区插件市场：浏览 awesome-dsh-plugin.com 目录，从 设置 → 插件 → 插件市场 安装/卸载插件到 profile。
- [siweina/dsh-novel-writer](https://github.com/siweina/dsh-novel-writer) — 小说写作助手：章节库管理、句式模式分析（九类句式/情感曲线/风格指纹）、风格自检、伏笔登记、批量导入与续写辅助，带 Web UI 开关。
- [taxueseek/argo](https://github.com/taxueseek/argo) — 专为 agent 打造的搜索工具：多语言，覆盖中文/英文/学术/代码/购物/金融/新闻/百科。
- [THU-MAIC/dsh-openmaic](https://github.com/THU-MAIC/dsh-openmaic) — OpenMAIC 教学：课堂、幻灯片、交互组件与苏格拉底式教学。
- [TonyDua/dsh-web-search-exa](https://github.com/TonyDua/dsh-web-search-exa) — ctx.web 接缝的零配置 Exa 网页搜索提供方：无 API key 时走匿名 MCP 兜底，配 key 时走 REST 搜索。
- [vibeinging/dsh-tool-search](https://github.com/vibeinging/dsh-tool-search) — 按 agent 的按需工具发现与渐进式 schema 披露。
- [xiaoyuyu6420/dsh-backup](https://github.com/xiaoyuyu6420/dsh-backup) — 一键备份 DSH 用户数据：/backup 命令、定时自动备份、sha256 校验与自动轮换。
- [xiehuan123/coding-coach](https://github.com/xiehuan123/coding-coach) — Coding Coach 编程教练：面向非开发人员的 35 技能 bundle + 完整 Agent 预设（八段编排流水线 + 工程/产品/界面技能），npm 可装 `dsh plugin add coding-coach`，同时提供 Claude Code 插件。
- [xiehuan123/dsh-deepread](https://github.com/xiehuan123/dsh-deepread) — DeepRead 精读助手：五种精读模式（quick / deep / map 知识地图（四档置信度）/ feynman 费曼读书法 / book 全书）、批量对比、预算预检与后台任务进度透明、微信公众号链接 / .pdf 文件（内置纯 JS 提取器）/ 粘贴文本，可选导出 MD / FreeMind 思维导图（XMind 可导入）/ 编辑风网页报告。
- [xmutfyh/dsh-plugin-writing-guard](https://github.com/xmutfyh/dsh-plugin-writing-guard) — 论文写作守卫：本地规则扫描修改过程残留、防御性写作与 AI 写作痕迹（破折号滥用、不是X而是Y、LLM 高频词、三连排比），论文文件写入后增量自动审计（writing_audit / writing_rules）。
- [yangyunsong023/dsh-sxs-anti-bot-http](https://github.com/yangyunsong023/dsh-sxs-anti-bot-http) — 反爬 HTTP 工具：UA 池轮换、指数退避重试、反爬墙检测（验证码/安全验证）与自适应限流，提炼自 SXS 生产采集体系（每日数百万请求）——工具：`sxs_fetch` / `sxs_fetch_json` / `sxs_rate_status`。
- [yangyunsong023/dsh-sxs-news-collector](https://github.com/yangyunsong023/dsh-sxs-news-collector) — 时事热点采集：一次调用聚合百度热搜 / 头条热榜 / 抖音热点 / 微博热搜（微博可选 cookie），返回标题+热度值，供内容创作借势——工具：`sxs_news_hot`。
- [ylwl1997/noatmark-dsh-plugin](https://github.com/ylwl1997/noatmark-dsh-plugin) — 文本卫生 dsh 插件：净化不可信文本、扫描隐形字符、清洗 LLM 格式、转义 CSV 公式注入。
- [ysr666/dsh-vision-router](https://github.com/ysr666/dsh-vision-router) — 为纯文本 Agent 提供视觉能力：内置免 Key 视觉链 + 像素级视觉工具（看图问答、定位、裁剪、像素对比、取色、OCR、矢量化、抠图、截图）；粘贴图片即可用。
- [zhaoolee/notes](https://github.com/zhaoolee/notes) — 将 DSH 对话导出为锤子便签风格 PNG，或在配置的账号工作区中新建和更新 Markdown 便签。
- [zimai233/dsh-adhd-copilot](https://github.com/zimai233/dsh-adhd-copilot) — ADHD 行为辅导技能：任务拆解、事项过载管理、启动仪式与失败重启。
- [zimai233/dsh-exam-countdown](https://github.com/zimai233/dsh-exam-countdown) — 查询 64 场中国考试（高考/考研/四六级/CPA/法考…）的规则日期（第二个周六、第一个周日）与倒计时。
- [zimai233/dsh-figma-to-lottie](https://github.com/zimai233/dsh-figma-to-lottie) — 将 SVG 路径与关键帧参数编译成自包含的 Lottie JSON 动画文件。
- [zimai233/dsh-image-search](https://github.com/zimai233/dsh-image-search) — 多引擎反向识图聚合：Google Lens、百度、Yandex、TinEye、SauceNAO、IQDB、Ascii2d。
- [zimai233/dsh-video-downloader](https://github.com/zimai233/dsh-video-downloader) — 检测并下载 B站/YouTube/抖音/小红书视频媒体，带清晰度与格式分析。
- [zimai233/dsh-wash-calendar](https://github.com/zimai233/dsh-wash-calendar) — 基于纯日期数学的周期习惯排程：下次发生日、区间排程与逾期提醒。
- [ZK-Andy/dsh-continual-evolve](https://github.com/ZK-Andy/dsh-continual-evolve) — 持续自进化：从会话轨迹沉淀版本化、可审计、可回滚的 harness 状态（提示词/记忆/技能/子代理规格），带审查门禁与技能热加载。
- [zp-home/dsh-recommend](https://github.com/zp-home/dsh-recommend) — DSH 插件透明排行与推荐：每日自动抓取 `dsh-plugin` 话题生态，公开评分模型，提供 rank/search/recommend 工具与设置页榜单。

### 🧩 技能包
- [creght-dev/skills](https://github.com/creght-dev/skills) — Creght 平台建站技能包：CLI 拉取/推送同步、页面与组件规范、CMS、表单、Auth、SEO、发布与版本回滚。
- [dhicoc/dsh-reverse-skill](https://github.com/dhicoc/dsh-reverse-skill) — 完整 reverse-skill 技能包（85 个 SKILL.md）的 DeepSeek Harness 插件：面向逆向工程、授权渗透测试与安全研究的技能路由包。
- [gongyijie85/dsh-ponytail](https://github.com/gongyijie85/dsh-ponytail) — 最懒资深工程师模式（Ponytail）的 DSH 移植：6 个技能（ponytail、ponytail-audit、ponytail-debt、ponytail-gain、ponytail-help、ponytail-review），改编自 DietrichGebert/ponytail（MIT）。
- [gongyijie85/mattpocock-skills-dsh](https://github.com/gongyijie85/mattpocock-skills-dsh) — Matt Pocock 完整发布技能集（25 个 SKILL.md：grilling、writing-for-agents、wait-what、TDD、code-review、wayfinder、ask-matt 路由等）的 DeepSeek Harness 插件：改编自 mattpocock/skills（MIT）。
- [gongyijie85/mattpocock-skills-dsh-zh](https://github.com/gongyijie85/mattpocock-skills-dsh-zh) — Matt Pocock 技能中文版的 DeepSeek Harness 插件：25 个 SKILL.md 正文全译中文（技术术语保留英文并附注释），改编自 mattpocock/skills（MIT）。
- [gwrsfsfeefdsfs/dsh-skill-curator](https://github.com/gwrsfsfeefdsfs/dsh-skill-curator) — DSH skill 经验回流与知识积累元技能：其他 skill 出问题解决后自动回流解决方案并登记知识库（关键词 + 本地 bge 语义双通道检索、7 项写回判断清单、防臃肿归档），附自校验与事件钩子工具。
- [docgen](https://github.com/JohnXu22786/docgen) — 文档工坊技能包：纯提示词文档生成——README、PR 描述、changelog 与代码审查。
- [skill-framework](https://github.com/JohnXu22786/skill-framework) — Praxis：面向 dsh 的工程方法论技能库（Agent Skills），以 Cordis 插件形式经 ctx.skills 提供。
- [skill-manager](https://github.com/JohnXu22786/skill-manager) — 多区域技能发现、渐进式披露、创建向导、审计与统计。
- [spec-driven](https://github.com/JohnXu22786/spec-driven) — keel（龙骨）：规格驱动开发纪律技能包——先立规格、验证假设、防止过度工程与范围蔓延。
- [leechen298/Code2Skill](https://github.com/leechen298/Code2Skill) — 从现有代码生成 Function、MCP、Agent Skill 和离线测试包，并作为可安装的 DSH Bundle 分发。
- [yanglaofish/dsh-skill-manager](https://github.com/yanglaofish/dsh-skill-manager) — DSH 技能生命周期管理插件：全局 / 工作区 / 会话三层模型下查看、编辑、导入、启用/停用技能，设置页与对话页统一管理界面，支持跨层全文搜索与分页。

### 🔁 工作流与自动化
- [940842546/dsh-permissions](https://github.com/940842546/dsh-permissions) — Claude Code 风格权限规则引擎：hard/deny/ask/allow 四级规则（hard 高于全访问、不可豁免）、workspace 作用域、通配符路径保护、可视化草稿式编辑器，规则持久化于 settings.yaml。
- [940842546/dsh-usage-billing](https://github.com/940842546/dsh-usage-billing) — 用量与消费统计：8/17 调价前后峰谷计费，主界面汇总面板、按会话明细与用量热力图。
- [biociao/dsh-science](https://github.com/biociao/dsh-science) — 面向 DSH 的 Claude Science 式科研工作台：ReAct 研究循环引擎（research_* 工具）、带溯源的版本化工件（artifact_* 工具）与面向基因组/病原体/生物信息的 10 个科研技能。
- [btspoony/dsh-advisor](https://github.com/btspoony/dsh-advisor) — 搭配一个副模型，每轮被动审查并注入见解。
- [btspoony/mstar-harness](https://github.com/btspoony/mstar-harness) — 技能驱动的 harness/loop 工程化工作流插件。
- [dsh-plan-execute](https://github.com/dsh-external/dsh-plan-execute) — plan/execute 双模型路由：规划模型思考、执行模型干活。
- [EvilIrving/dsh-proof](https://github.com/EvilIrving/dsh-proof) — 独立只读验收层：顶层 turn 收尾前 spawn 只读 verifier，未通过时把缺口注回主 agent。
- [fakechris/dsh-track](https://github.com/fakechris/dsh-track) — 嵌入式任务管理引擎：决策点协议、念头捕获墙、Linear 形 issue 存储。
- [fuhefei/dsh-sentinel](https://github.com/fuhefei/dsh-sentinel) — 条件驱动唤醒：file/command/http/process/webhook 持久监视，触发即唤醒 agent。
- [huchunlinnk/deepseek-desk-rsi](https://github.com/huchunlinnk/deepseek-desk-rsi) — Recursive Self-Improvement engine: bounded perceive→integrate→verify→parity→repair→propose loop + 128-plugin 1:1 parity gate — DSH maintains DSH.
- [icetomoyo/dsh_workflow](https://github.com/icetomoyo/dsh_workflow) — 把 UltraCode 式多 Agent 调度带给 DSH：可生成、可保存、可治理、可观察、可恢复的 Workflow 层。
- [Jesse-njx/dsh-routines](https://github.com/Jesse-njx/dsh-routines) — 定时 Agent：按 cron 计划运行 prompt，把摘要送到你已有的地方，内置重叠/漏跑/超时安全策略。
- [file-planning](https://github.com/JohnXu22786/file-planning) — trailmap：磁盘持久化执行规划——里程碑状态机、依赖标注、审计事件与复盘纪要。
- [task-board](https://github.com/JohnXu22786/task-board) — 跨会话事件溯源工作台账：任务跟踪、审计历史、看板导出。
- [Letter2025/dsh-approval-llm](https://github.com/Letter2025/dsh-approval-llm) — 基于模型的权限审批：由独立审查模型自动应答 approval 权限请求。
- [Letter2025/dsh-model-failover](https://github.com/Letter2025/dsh-model-failover) — 两级模型熔断与回退：模型或平台连续失败后自动熔断，并把下一个请求路由到配置好的备用模型。
- [lonelymoon87/dsh-specflow](https://github.com/lonelymoon87/dsh-specflow) — 增加规格工件、技能、命令、由 goal 驱动的实施流程和任务进度上下文。
- [NanmiCoder/dsh-agent-teams](https://github.com/NanmiCoder/dsh-agent-teams) — AgentTeams 多智能体团队。
- [omdsh-dev/dsh-deep-research](https://github.com/omdsh-dev/dsh-deep-research) — 自适应深度研究编排器（基于官方 workflow 引擎）。
- [omdsh-dev/dsh-inspect](https://github.com/omdsh-dev/dsh-inspect) — 发现问题→修复交付→质量复查的对抗式闭环工具集。
- [odai-dsh-plugin](https://github.com/orziz/odai/tree/main/dsh/plugin) — 面向整个 DSH profile 的治理与路由 bundle，提供可配置的压缩调用与本地作用域语义记忆；兼容 DSH 0.1.0-rc.6 与 0.1.0-rc.7。
- [PerryLink/dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) — 工程纪律守门：动笔前审讯需求，红绿测试证据门，交付后对抗评审（grill-requirements 技能 + 工具策略门）。
- [Sev7een/dsh-plugin-automations](https://github.com/Sev7een/dsh-plugin-automations) — 设置页定时任务：支持准点或 DeepSeek 谷时段执行、单次/每日重复，并持久化任务状态。
- [timwhitez/dsh-self-evolving](https://github.com/timwhitez/dsh-self-evolving) — 证据优先、可崩溃恢复的自进化引擎：有界生成 Cordis 候选插件、一次性真实 Loader 准入、Harbor 评估，并保留可审计的日志化谱系。
- [titanwings/dsh-automation](https://github.com/titanwings/dsh-automation) — 定时任务：让 Coding 任务按计划在全新 Agent Session 中运行，保留可审计历史。
- [titanwings/dsh-plannotator](https://github.com/titanwings/dsh-plannotator) — 计划批注：选中计划原文逐条批注，结构化反馈送回 Agent。
- [vlln/dsh-loop](https://github.com/vlln/dsh-loop) — 定时循环：`/loop` 命令 + loop 工具 + 活动状态条。

### 🔔 通知与集成
- [Andyqwe44/dsh-notify-win](https://github.com/Andyqwe44/dsh-notify-win) — 原生 Windows toast + 任务栏闪烁，任务完成/审批/提问时触发，支持 Win10/11，npm 安装 `dsh plugin --profile web add dsh-notify-win`。
- [BiBoyang/dsh-im-bridge](https://github.com/BiBoyang/dsh-im-bridge) — 微信（iLink）双向桥：turn 完成/批准请求推送、聊天内批准与消息注入、持久去重与长回复收敛分段；通道层为多 IM 预留。
- [bill9109/dsh-web-ui-notify](https://github.com/bill9109/dsh-web-ui-notify) — 桌面通知提醒。
- [bill9109/dsh-webbridge](https://github.com/bill9109/dsh-webbridge) — DSH 结合 Kimi WebBridge。
- [bobleer/dsh-acp-for-bitfun](https://github.com/bobleer/dsh-acp-for-bitfun) — BitFun 与 DSH 的 ACP 交互对接。
- [cdxiaodong/dsh-island](https://github.com/cdxiaodong/dsh-island) — 通过 Unix socket 把 DSH agent 的会话、工具调用与审批实时桥接到 CodeIsland macOS 刘海面板，可直接在面板上批准/拒绝。
- [dingyi222666/dsh-session-notification](https://github.com/dingyi222666/dsh-session-notification) — 会话完成等四种状态的通知响应，支持浏览器提示。
- [dsh-feishu](https://github.com/PGZXB/dsh-feishu) — DeepSeek Harness 的飞书 UI：面板驱动控制台，卡内审批与提问，流式卡片，扫码一键配置。
- [dsh-feishu-notify](https://github.com/dsh-external/dsh-feishu-notify) — 飞书通知（会话结束/等待输入）。
- [dsh-opencode-server](https://github.com/dsh-external/dsh-opencode-server) — 通过 opencode attach 获得丝滑 TUI。
- [imetn/dsh-lark-bridge](https://github.com/imetn/dsh-lark-bridge) — DeepSeek Harness 的飞书/Lark 双向控制器，支持 Project 与 Session 路由、交互卡片、审批、附件和任务控制。
- [Jesse-njx/dsh-chatnode-wechat](https://github.com/Jesse-njx/dsh-chatnode-wechat) — 通过 iLink 网关在微信里与 DSH agent 聊天、监控与审批：双向文本、会话切换、进度摘要与编号审批提示。
- [notifier](https://github.com/JohnXu22786/notifier) — dsh-chime：桌面信号插件——任务完成、等待批准或出错时发送通知与提示音。
- [Laplace-bit/dsh-bell-notify](https://github.com/Laplace-bit/dsh-bell-notify) — 生命周期铃声与状态点：为每个环节合成专属提示音（Web Audio，零音频文件），右下角呼吸状态点显示工作状态。
- [LoserFox/telegram](https://github.com/LoserFox/telegram) — Telegram Bot API 桥接：长轮询、per-chat 会话、HTML 格式化。
- [omdsh-dev/dsh-notification](https://github.com/omdsh-dev/dsh-notification) — 回合完成桌面通知，按结果分控 + 关键词过滤。
- [omdsh-dev/dsh-open-in-vscode](https://github.com/omdsh-dev/dsh-open-in-vscode) — 从 Web GUI 一键在 VS Code 中打开工作区目录。
- [openma-ai/deepseek-harness-acp](https://github.com/openma-ai/deepseek-harness-acp) — ACP profile 插件与独立 stdio server，可从 Zed 等 ACP 客户端使用完整 DSH agent，并共享 DSH 凭据与会话。
- [SeverusZh/dsh-notify-windows](https://github.com/SeverusZh/dsh-notify-windows) — Windows 通知，零依赖。

### 🔌 模型与账号接入
- [btspoony/dsh-llm-fallbacks](https://github.com/btspoony/dsh-llm-fallbacks) — 基于角色的模型重试与备用策略。
- [dsh-vision](https://github.com/dsh-external/dsh-vision) — 视觉桥接：view_image 工具接任意 OpenAI 兼容 VLM。
- [dylan121322/llm-adaptive](https://github.com/dylan121322/llm-adaptive) — 自适应模型路由：请求级复杂度分类，按配置链自动选择后端 provider。
- [franksong2702/dsh-codex-connect](https://github.com/franksong2702/dsh-codex-connect) — 通过 ChatGPT OAuth 将 OpenAI Codex 模型接入 DeepSeek Harness，并提供可选的搜索与图片工具。
- [model-catalog](https://github.com/JohnXu22786/model-catalog) — 模型目录自动发现：从 OpenAI 兼容主机获取模型列表、价格与能力，归一化为即用配置。
- [kam74515-boop/dsh-everything-oauth](https://github.com/kam74515-boop/dsh-everything-oauth) — 把本机 Codex / Grok / Claude / OpenCode / CC Switch 登录态导入 DSH，在设置里自选来源并启用模型。
- [omdsh-dev/Qwen-MM-Plugins](https://github.com/omdsh-dev/Qwen-MM-Plugins) — Qwen 多模态插件支持。
- [suntianc/dsh-codex-auth](https://github.com/suntianc/dsh-codex-auth) — 复用 Codex CLI 的 ChatGPT 登录态注册 `openai-codex` LLM 路由，并在 DSH Web 设置中提供 GPT Auth 控件。
- [tianxia--/dsh-llm-local-token](https://github.com/tianxia--/dsh-llm-local-token) — 复用本机 Codex CLI 与 Claude Code 的 OAuth 凭据注册 OpenAI Codex 和 Anthropic 模型路由，并在 Web 中显示订阅用量。

### 🧑‍💻 开发与运行时
- [030611/dsh-telemetry-redactor](https://github.com/030611/dsh-telemetry-redactor) — 在已配置遥测后端接收前，对 `session-telemetry/record` 导出副本中的已支持秘密模式进行脱敏。
- [030611/dsh-verification-receipt](https://github.com/030611/dsh-verification-receipt) — 把每轮工具计数与粗粒度验证信号写入本地 JSONL，不保存提示词、工具参数或结果正文。
- [15828148/dsh-portable-launcher](https://github.com/15828148/dsh-portable-launcher) — Windows 一键便携启动器，国内镜像回退。
- [Areium/dsh-fail-logger](https://github.com/Areium/dsh-fail-logger) — 全模式调用工具失败自动实录：把原生工具 / PTC run_code / 代码内嵌工具调用的失败错因去重计数后写入 skill，越用越少错。
- [arrow949/dsh-turn-approval](https://github.com/arrow949/dsh-turn-approval) — DSH「允许本次任务」临时授权：仅在当前任务内自动放行同类 `danger-full-access` 请求，任务结束自动失效。
- [asdf17128/dsh-doctor](https://github.com/asdf17128/dsh-doctor) — Profile 体检：检出 patch 丢失字段、不存在的 entry id 与工具重名冲突。
- [BiBoyang/dsh-eval-harness](https://github.com/BiBoyang/dsh-eval-harness) — DSH 插件评测框架：YAML 用例驱动真实 headless agent，断言工具调用/参数/返回与 token 用量，baseline 门禁做 CI 回归。
- [BrambleXu/dsh-annotate](https://github.com/BrambleXu/dsh-annotate) — 面向 Vibe Coding 的浏览器元素标注插件：直接选取页面元素，并将结构化视觉反馈发送给 DeepSeek Harness Agent。
- [BrambleXu/dsh-prompt-profile](https://github.com/BrambleXu/dsh-prompt-profile) — DeepSeek Harness 可复用 Markdown Prompt Profile，支持单轮模型选择、参数替换和状态恢复。
- [BrambleXu/dsh-revdiff](https://github.com/BrambleXu/dsh-revdiff) — DeepSeek Harness 原生交互式 Git diff 审查，支持结构化批注并回传当前 Agent 会话。
- [cdxiaodong/dsh-guardian](https://github.com/cdxiaodong/dsh-guardian) — Agent 安全护栏：拦截并审计所有工具调用，命中敏感操作就要求人工确认。
- [CH4ACKO3/dsh-harmony](https://github.com/CH4ACKO3/dsh-harmony) — 让一个 DSH 插件在运行时修改另一个插件的代码，并提供 Patch 排序、冲突检查和热重载。
- [DietCokewithSugar/dsh-user-experience](https://github.com/DietCokewithSugar/dsh-user-experience) — 帮你发现项目中可能存在的用户体验问题：自动走查 React/TypeScript 源码，定位问题并给出具体优化建议。
- [disyli/dsh-tool-call-stats](https://github.com/disyli/dsh-tool-call-stats) — 进程内工具调用统计：提供 `tool_stats` 工具，按工具汇报调用次数、失败次数与平均耗时。
- [DoggyHU/dsh4vscode](https://github.com/DoggyHU/dsh4vscode) — 基于 DSH agent 的 VS Code 聊天窗口，模型自动路由。
- [EvilIrving/dsh-repro](https://github.com/EvilIrving/dsh-repro) — /repro 导出最小可复现问题包：去 secret 的会话日志、失败命令与 git diff。
- [foolgry/dsh-desktop](https://github.com/foolgry/dsh-desktop) — 开箱即用的 Electron 桌面版，自动跟随上游发版。
- [forrestchang/dsh-multica-runtime](https://github.com/forrestchang/dsh-multica-runtime) — 让 dsh 运行时跑在 Multica 上。
- [fountunt/dsh-session-cleaner](https://github.com/fountunt/dsh-session-cleaner) — 无需重启即可删除运行中 Web 运行时里的会话。
- [hust-open-atom-club/oh-dsh](https://github.com/hust-open-atom-club/oh-dsh) — 社区发行版：TUI、桌面端与 Web UI 统一体验，分层安装、一步到位。
- [hyqhyq3/dsh-mcp-manager](https://github.com/hyqhyq3/dsh-mcp-manager) — MCP 服务器管理器：OAuth 或静态 token 认证 + 设置页。
- [ICCuse/dsh-pain-point-check](https://github.com/ICCuse/dsh-pain-point-check) — 强制痛点检查：同一问题连续 2 个实验未收敛后注入三问、拦截非调查类工具调用直到答出、阻止同方向重试。
- [ilharp/dsh-tool-approval](https://github.com/ilharp/dsh-tool-approval) — 手动审批模式（Manual/Ask Mode）。
- [Jayden-X-L/forkprobe](https://github.com/Jayden-X-L/forkprobe) — 同一任务并行试跑多个技能，对比结果选出最优。
- [Jesse-njx/dsh-plugin-manager](https://github.com/Jesse-njx/dsh-plugin-manager) — `dsh pm` 插件管理器：多源搜索（awesome 列表 + GitHub + npm）、按 profile 安装/移除/更新，以及 doctor 审计（清单、bundle patch、版本漂移）。
- [Jesse-njx/dsh-plugin-manager-registry](https://github.com/Jesse-njx/dsh-plugin-manager-registry) — 离线容错的插件注册表，聚合并去重各类来源的 DSH 插件。
- [Jesse-njx/dsh-polyglot](https://github.com/Jesse-njx/dsh-polyglot) — DSH 的模型切换器：指向任意 OpenAI 兼容端点，内置精选免费/低价 DeepSeek 服务商预设，免费额度限流时自动回退。
- [Jesse-njx/dsh-tmuxctl](https://github.com/Jesse-njx/dsh-tmuxctl) — 掌控你的 tmux 面板：list/send-keys/capture、在面板中运行长任务并 watch，破坏性命令需审批。
- [hooks-adapter](https://github.com/JohnXu22786/hooks-adapter) — 通用 hooks 兼容层：在 dsh 上运行 Claude Code / Codex / opencode 配置中声明的 hooks。
- [Leon0555/dsh-lan-access](https://github.com/Leon0555/dsh-lan-access) — 局域网访问：Web GUI 绑定 0.0.0.0 + crypto.randomUUID polyfill（修复非安全上下文下 RPC 崩溃）。
- [Lixiaoyiao/deepseek-harness-action](https://github.com/Lixiaoyiao/deepseek-harness-action) — GitHub Action 运行 DSH 做 PR 审查、CI 诊断与受信任修复。
- [lonelymoon87/dsh-gitflow](https://github.com/lonelymoon87/dsh-gitflow) — 增加需要审批的 Git 状态、diff、日志、提交、分支和可选检查点工具。
- [lonelymoon87/dsh-guardian](https://github.com/lonelymoon87/dsh-guardian) — 增加危险操作策略检查、输出脱敏和安全审查工作流。
- [LoserFox/dsh-git-identity](https://github.com/LoserFox/dsh-git-identity) — git 提交固定使用环境自身作者身份，环境变量注入压过一切 `git config` 设置。
- [omdsh-dev/dsh-plugin-check](https://github.com/omdsh-dev/dsh-plugin-check) — 插件健康检查：扫描清单协议/patch 格式/构建陷阱，零依赖只读。
- [omdsh-dev/dsh-security-audit](https://github.com/omdsh-dev/dsh-security-audit) — 本机安全审计：配置/插件来源/会话/网络暴露面，只读脱敏风险报告。
- [omdsh-dev/dsh-session-health](https://github.com/omdsh-dev/dsh-session-health) — 会话文件帧级扫描诊断（torn/损坏/空会话检测）。
- [omdsh-dev/fabric](https://github.com/omdsh-dev/fabric) — 类似 MC Fabric 的 hook 处理器。
- [omdsh-dev/plugin-template](https://github.com/omdsh-dev/plugin-template) — 插件模板仓库（基于 turtle-ui 官方仓库）。
- [omdsh-dev/sandbox-micro](https://github.com/omdsh-dev/sandbox-micro) — microsandbox 沙箱支持。
- [omdsh-dev/sandbox-mxc](https://github.com/omdsh-dev/sandbox-mxc) — 微软跨平台沙盒支持。
- [omdsh-dev/sandbox-nono](https://github.com/omdsh-dev/sandbox-nono) — nono 沙盒支持。
- [PerryLink/dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) — 官方 MCP 客户端（dsh-mcp-client）的只读运行时管理面板：/mcp 命令与设置页 MCP 页签展示连接状态、已注册工具、错误与重连计数，脱敏展示并提供启停 patch 建议。
- [ruimin251204/dsh-plugin-surgery](https://github.com/ruimin251204/dsh-plugin-surgery) — 插件手术刀：安全卸载（dry-run 预览影响面、快照、三方对账、失败自动回滚）、一键回滚、restart-pending 确认与插件体检。
- [slywalker2006/dsh-passwords](https://github.com/slywalker2006/dsh-passwords) — DSH Web UI 登录网关：首次配置、bcrypt + 静态加密（AES-256-GCM/HMAC）、防爆破、审计日志、TLS 1.2+ 与 80→443 跳转、CSRF 与防嵌框。
- [Small-tailqwq/dsh-tps](https://github.com/Small-tailqwq/dsh-tps) — TPS 指标插件。
- [suimi8/dsh-test-runner](https://github.com/suimi8/dsh-test-runner) — 结构化测试运行工具：自动识别 Vitest/Jest/pytest/node:test 并解析失败。
- [vibeinging/dsh-agent-budget](https://github.com/vibeinging/dsh-agent-budget) — agent 树 token 预算管理。
- [vibeinging/dsh-trace](https://github.com/vibeinging/dsh-trace) — 遥测后端：把 turns、model steps、tool calls 导出到 yiTrace。
- [vlln/plugin-registry](https://github.com/vlln/plugin-registry) — 插件生态基建：浏览器面板管理官方 repository 插件（0 patch）+ make-dsh-plugin 插件开发引导技能。
- [william-jin-cmu/dsh-evolve](https://github.com/william-jin-cmu/dsh-evolve) — 自进化：agent 在会话内给自己热挂载/卸载持久化插件。
- [wuxiangru915/dsh-review-loop](https://github.com/wuxiangru915/dsh-review-loop) — 增量 diff 审查器：Web 审查面板 + 审查意见注入 agent。
- [xgone/dsh-remote](https://github.com/xgone/dsh-remote) — DeepSeek Harness 网页端远程访问与认证：账号/密码登录门、MFA（TOTP 两步验证）、签名会话 Cookie、基于角色的访问控制、浏览器内目录选择器，以及账号管理设置页。
- [xingyingyuzhui/dsh-updater-ui](https://github.com/xingyingyuzhui/dsh-updater-ui) — 设置页中的 DSH 自助更新器：一键检查/拉取（git pull --ff-only）、自动后台检查、版本对比与更新说明预览，带红点提醒。
- [yflmq001/dsh-cost-tracker](https://github.com/yflmq001/dsh-cost-tracker) — 按模型追踪 token 成本：可配置缓存命中/未命中、输出与高峰时段单价，实时会话花费条，并标记未配置价格的模型。
- [Yuuz12/dsh-webui-auth](https://github.com/Yuuz12/dsh-webui-auth) — WebUI 身份认证：HTTP/传输层强制登录（资源、插件 bundle、/api、WebSocket 四层防护），服务端会话 + HttpOnly Cookie。
- [Zhenyu98/dsh-context-doctor](https://github.com/Zhenyu98/dsh-context-doctor) — 上下文注入审计：统计指令链/技能目录/工具 schema 的 token 成本，检测重复与冲突。

### 🎮 娱乐
- [AnacondaKC/dsh-douyin](https://github.com/AnacondaKC/dsh-douyin) — 侧栏短视频：原生播放器、系列导航、精确历史回放。
- [AnacondaKC/dsh-stock-market](https://github.com/AnacondaKC/dsh-stock-market) — 有效解决了写代码的时候账户不能同时亏钱的 BUG。
- [anweat/dsh-browser](https://github.com/anweat/dsh-browser) — 自包含浏览器运行时：Playwright（chromium）+ OpenCLI 作为插件本地依赖（全局复用回退），提供 `browser` 服务与 9 个交互式浏览器工具。
- [anweat/dsh-restart](https://github.com/anweat/dsh-restart) — DSH 重启插件：可配置的重启方式（Node 原生/旧 PowerShell 适配）、重启后自动继续的提示词、可选看门狗自动拉起。
- [anweat/dsh-voice-webspeech](https://github.com/anweat/dsh-voice-webspeech) — 浏览器 Web Speech API 语音输入：零服务端、零密钥、零模型下载（Edge=Azure 语音、Chrome=Google 语音）。
- [anweat/dsh-web-search-pro](https://github.com/anweat/dsh-web-search-pro) — 增强型、可持久化的网页搜索：多引擎路由（DeepSeek/Exa/DDG/Bing/Jina + GitHub/B站/YouTube/V2EX/小红书/Twitter/Reddit/RSS）、SQLite+LRU 缓存、userscript 风格抽取、Playwright 渲染。
- [beancookie/dsh-plugin-nintendo](https://github.com/beancookie/dsh-plugin-nintendo) — 基于 jsnes 的 NES 模拟器：独立弹窗游玩、快捷键开关，Agent 可调用 `nes_play` 工具加载 ROM，支持存档/读档/截图。
- [dsh-ui-whale](https://github.com/dsh-external/dsh-ui-whale) — 像素鲸鱼伙伴（眨眼/摆尾/喷水/爱心）。
- [FlytoMAYDAY80/dsh-pet](https://github.com/FlytoMAYDAY80/dsh-pet) — 桌面小鲸鱼，实时感知会话状态。
- [hellodigua/dsh-emoji](https://github.com/hellodigua/dsh-emoji) — 为 AI 回复自动添加表情。
- [HuanLinOTO/dsh-plugin-d399](https://github.com/HuanLinOTO/dsh-plugin-d399) — 模型生成时弹出小游戏菜单（wordle/消消乐，可扩展）。
- [JAdpp/dsh-whale-galgame](https://github.com/JAdpp/dsh-whale-galgame) — 多角色 Galgame 对话界面：角色与回复模型可独立切换，分角色保存好感度、记忆、对话历史与 CG 图鉴，并根据 Harness 跨会话任务事件做出角色回应。
- [lhh010/dsh-minigames](https://github.com/lhh010/dsh-minigames) — 右侧小游戏面板：18 款离线小游戏，等模型回复时的摸鱼神器。
- [minybear/DeepSeek-Harness-Pet](https://github.com/minybear/DeepSeek-Harness-Pet) — Codex 风格桌面宠物：右下角悬浮动画精灵，随 agent 运行状态实时变化（工作、等待、报错、完成）。
- [Moeblack/deepseek-manners](https://github.com/Moeblack/deepseek-manners) — 给每次消息后注入感谢语，做个有礼貌的人。
- [Nagi-ovo/dsh-ads](https://github.com/Nagi-ovo/dsh-ads) — 2005 年中文站点风格的整活广告插件：侧栏广告/信息流/角落弹窗 + 假关闭叉，素材全虚构。
- [omdsh-dev/dsh-auto-chess](https://github.com/omdsh-dev/dsh-auto-chess) — 自走棋：人机对战或双 AI 对弈。
- [omdsh-dev/dsh-gomoku](https://github.com/omdsh-dev/dsh-gomoku) — 与 AI 下五子棋，也可让 AI 对局比棋力。
- [sunshine-lang/dsh-pdf](https://github.com/sunshine-lang/dsh-pdf) — PDF 工具箱：基于 pdfjs-dist 提取文本、元数据与页码范围。
- [sunshine-lang/dsh-weather](https://github.com/sunshine-lang/dsh-weather) — 天气工具：Open-Meteo 数据（免费，无需 API key）。
- [vlln/whale-girl](https://github.com/vlln/whale-girl) — 桌面宠物（QQ 宠物形态）：右下角悬浮、可拖拽/投喂/玩耍。
- [william-jin-cmu/dsh-stickers](https://github.com/william-jin-cmu/dsh-stickers) — 用户与 agent 双向表情贴纸互动。

## 相关

- [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) - 官方运行时与核心文档。
- [DeepSeek](https://deepseek.com) - 官方入口。
- [dsh-ops](https://github.com/MiraculousGarfield/dsh-ops) - dsh 运维工具箱：一键健康检查、配置快照/还原、服务看门狗与事故运维手册（纯本地脚本，无需 AI）。

## 贡献

欢迎提 PR 收录你的插件：在 `README.md` 和 `README.en.md` 的对应分类下各加一行，格式 `- [名称](链接) — 一句话描述`。

也请为你的插件仓库添加 [`dsh-plugin`](https://github.com/topics/dsh-plugin) topic，方便大家发现。

## 徽章

插件已被收录？欢迎在你的 README 里挂上徽章：

[![Awesome DSH Plugin](https://beancookie.github.io/awesome-dsh-plugin/badge.svg)](https://beancookie.github.io/awesome-dsh-plugin)

```markdown
[![Awesome DSH Plugin](https://beancookie.github.io/awesome-dsh-plugin/badge.svg)](https://beancookie.github.io/awesome-dsh-plugin)
```

## 免责声明

本项目是社区维护的索引。插件由各自作者开发与维护，收录不构成背书，亦不对任何插件的安全性、质量或维护状态作出保证。安装插件即在你的机器上运行第三方代码——请自行审阅源码、风险自担。本项目与 DeepSeek 无隶属关系。

本项目积极支持并感谢 [LINUX DO](https://linux.do) 社区——一个欢迎技术爱好者的温馨空间。
