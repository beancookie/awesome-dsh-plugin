# AGENTS.md

DeepSeek Harness（`dsh`）插件的精选列表（awesome list）。两个 README 是内容唯一来源，其余文件均由它们生成。

## 内容来源（source of truth）

- `README.md`（中文，GitHub 默认展示）与 `README.en.md`（英文）是唯一需要手动编辑内容的文件。二者必须保持同步：插件集合相同、分类相同、每个插件各占一行。
- 语言映射：`site/locales.mjs` 中 `zh` locale 的 `readme` 指向 `README.md`（中文内容）、`en` locale 指向 `README.en.md`（英文内容）——`zh` 是默认 locale（`x-default`），站点 `/` 为中文、`/en/` 为英文。改动时保持这个映射。
- `docs/`（生成的网站）、`data/npm-map.json`、`data/added-dates.json`、`data/stars.json` 都是自动生成的——切勿手动编辑。
- 插件计数行由构建脚本自动改写（`README.md` 用 `**N** 个插件`、`README.en.md` 用 `**N** plugins`），不要手动改动。

## 目录结构（每个文件夹的作用）

- `site/` — 网站源码：`template.html`（页面骨架，含 CSS 样式与前端交互 JS，用 `__TOKEN__` 占位）与 `locales.mjs`（语言与文案的唯一来源：分类名、标题、界面字符串）。build-site.mjs 据此生成页面。
- `scripts/` — 构建与探测脚本：`build-site.mjs`（解析两个 README，生成站点、`data/` 产物，按 owner/repo 字母序规范化 README 并同步计数）、`probe-npm.mjs`（探测各仓库对应的 npm 包，写入缓存）、`probe-stars.mjs`（探测各仓库 GitHub Star 数，写入缓存；需联网）、`check-order.mjs`（离线 lint：校验两 README 分类内插件是否按字母序）、`readme.mjs`（共享的解析与排序键，供 build-site / check-order 复用）。
- `docs/` — 生成的网站（GitHub Pages 部署目录）：`index.html`、各分类页、`plugins.json`、`sitemap.xml`、`feed.xml`、`logo.png`、`badge.svg`。自动生成，切勿手动编辑。
- `data/` — 自动生成的账本/缓存：`npm-map.json`（repo → npm 包映射）、`stars.json`（repo → GitHub Star 数与首次提交时间，供站点 Star/最新排序）与 `added-dates.json`（插件收录日期）。由脚本维护，切勿手动编辑。
- `images/` — 源素材：`logo.png`（站点与 README 使用的 logo 源文件）。
- `.github/` — GitHub 配置：`workflows/build-site.yml`（每 6 小时定时 + 推送 `main` 时自动构建并提交生成文件）、`workflows/pr-check.yml`（PR 时离线校验 README 排序）与 `pull_request_template.md`（PR 提交模板）。
- `.git/` — git 内部元数据，无需改动。

## 添加插件

每个插件占一行，由 `scripts/build-site.mjs` 中的严格正则解析：

```
- [owner/repo](https://github.com/owner/repo) - 以句号结尾的一句话描述。
```

- URL 必须是 `https://github.com/...`，其他域名不会被解析。
- 分类取自最近的 `###` 标题，标题必须包含 `site/locales.mjs`（`categories`）中对应的分类名。共 11 个固定分类（`ui`、`theme`、`session`、`memory`、`tools`、`skill`、`workflow`、`notify`、`model`、`dev`、`fun`）——不要新增分类，除非同时更新 `scripts/build-site.mjs` 中的 `CAT_IDS`。
- 必须在两个 README 的对应分类下各加同一行，否则 `build-site.mjs` 会报 `missing: <url>` 并失败。
- 分隔符为 ` - `（英文）或 ` — `（中文），解析器两者都接受。
- 分类内插件按 **owner/repo 字母序**（大小写不敏感）排列：`scripts/build-site.mjs` 每次构建会按此重排并回写两个 README，PR 经 `scripts/check-order.mjs` 校验。新行加在分类下任意位置即可，构建会自动排好。

## 整理流程（分类与数量）

### 分类

共 11 个固定分类，中英文名以 `site/locales.mjs`（`categories`）为准：

| id | 中文标题 | 英文标题 |
|----|----------|----------|
| ui | UI 增强 | UI Enhancements |
| theme | 主题与外观 | Themes & Appearance |
| session | 会话与消息 | Sessions & Messages |
| memory | 记忆 | Memory |
| tools | 工具与能力 | Tools & Capabilities |
| skill | 技能包 | Skills |
| workflow | 工作流与自动化 | Workflow & Automation |
| notify | 通知与集成 | Notifications & Integrations |
| model | 模型与账号接入 | Models & Providers |
| dev | 开发与运行时 | Development & Runtime |
| fun | 娱乐 | Just for Fun |

- 按插件核心功能归类：技能包/技能路由 → `skill`，UI/交互 → `ui`，主题 → `theme`，会话/消息 → `session`，记忆 → `memory`，工具/能力 → `tools`，工作流/自动化 → `workflow`，通知/集成 → `notify`，模型/账号 → `model`，开发/运行时 → `dev`，其余娱乐向 → `fun`。
- 同一插件在两个 README 必须放入对应分类（中文用中文标题、英文用英文标题），否则构建报 `missing: <url>` 失败。
- 不要新增分类；确需新增时同步更新 `scripts/build-site.mjs` 的 `CAT_IDS` 与 `site/locales.mjs` 的 `categories`。

### 数量

- 总数计数行由 `scripts/build-site.mjs` 自动改写：`README.md` 用 `**N** 个插件`、`README.en.md` 用 `**N** plugins`，切勿手动编辑。
- 站点里的分类计数、`docs/plugins.json` 的 `count`、JSON-LD 的 `numberOfItems` 均由构建脚本按解析到的条目自动计算，无需维护。
- 整理完成后依次运行 `node scripts/probe-npm.mjs`（需联网探测 npm 映射）与 `node scripts/build-site.mjs`，确认两个 README 计数与新增/移除插件数一致、`docs/` 重新生成。

## 需求（两条硬性要求）

### 1. 中英文翻译无缺失（双 README 逐条同步）

- 两个 README 必须逐条对齐：插件集合相同、分类相同、数量一致。任何插件都不得只出现在其中一个 README（即不允许存在「翻译缺失」）。
- 新增/删除/修改插件时，必须同步更新两个 README 的对应行；补翻译时中英文描述应一一对应。
- 校验：`scripts/readme.mjs` 的 `parseReadme` 可对比两 README 的 URL 集合（zh 与 en 各解析一次，取差集），`build-site.mjs` 在单侧缺失时也会报 `missing: <url>` 失败。

### 2. 插件按项目（owner/repo）字母序排序

- 分类内插件按项目标识排序：URL 去掉 `https://github.com/` 前缀与 `/tree/...` 后缀后的大小写不敏感字母序（即 owner/repo）。
- `scripts/build-site.mjs` 每次构建自动重排并回写两个 README，PR 由 `scripts/check-order.mjs` 离线校验；新行放分类内任意位置即可，构建会自动排好。

## 构建 / 验证

没有 npm scripts、测试或 lint。需要 Node 22（脚本使用 ESM、`fetch`、顶层 await）：

```
node scripts/probe-npm.mjs    # 探测 npm 仓库（需联网；失败时不会改动缓存）
node scripts/probe-stars.mjs  # 探测 GitHub Star 数与首次提交时间（需联网；可用 GITHUB_TOKEN 提升配额）
node scripts/build-site.mjs   # 重新生成 docs/ 与 data/，按字母序规范化 README 并同步计数
node scripts/check-order.mjs  # 离线校验：两 README 分类内插件是否按 owner/repo 字母序
```

先跑 probe，再跑 build。CI（`.github/workflows/build-site.yml`）在推送 `main` 时与每 6 小时定时会依次运行两者并自动提交生成的文件——所以不要手动提交 `docs/`/`data/`；注意 CI 只在 `main` 分支触发，PR 分支不会触发。

## 收录规则（见 contributing.md）

- 被收录的插件必须在 `package.json` 中声明 `dsh.bundle` manifest（仅有 `dsh.client` 不行），否则无法安装。
- 描述只说明插件功能——不加营销词/最高级措辞；以句号结尾。
- 仓库应打上 `dsh-plugin` topic。
