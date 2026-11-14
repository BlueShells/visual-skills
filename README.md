# Visual Skills

精选的 Claude Code / Agent Skills 视觉与仿真技能：把流程、机器、工厂、科学机制变成可交互的单文件 HTML、图表或动画。每个技能都附来源、安装方式、用法和产出说明。

## 技能一览

| 技能 | 适合 | 产出 | 安装 |
|---|---|---|---|
| [TinyCharts](skills/01-tinycharts.md) | 流程、教学、结构演示；28 种手绘 2.5D 风格 | 可点击、可回放的手绘风图表 | 官网获取；终端一行命令或 `.skill` 上传 |
| [teardown](skills/02-teardown.md) | 大型/仿生机械拆解、3D 可交互讲解 | 单文件 HTML 3D 拆解模拟器 + MP4 | `npx skills add elvarofficial/teardown -g -a claude-code` |
| [factory-skill](skills/03-factory-skill.md) | 微缩 3D 工厂流水线、离散事件仿真 | 单文件 HTML 倾斜移轴工厂 + HUD | `npx skills add AirsupHQ/factory-skill -g -a claude-code` |
| [machine-skill](skills/04-machine-skill.md) | 重型机械、高拟真可交互 3D 网页 | 单文件 HTML 物理仿真 + 成片 | `npx skills add AirsupHQ/machine-skill -g -a claude-code` |
| [SeeCode](skills/05-seecode.md) | 流程、硬件、架构可视化；动画图 | 单文件 HTML，可导出 SVG/PNG/GIF/MP4 | `/plugin marketplace add Aryanutkarsh/seecode` 或 `npx skills add Aryanutkarsh/seecode -g` |
| [anatomy](skills/06-anatomy.md) | 线稿风机械运转、零件拆解、技术概念 | 等距 SVG/WebGL/3D 可交互图 | `npx skills add wheresryan22/anatomy -g` |
| [anima](skills/07-anima.md) | 生物/化学机制、教学科普演示 | 带引用的交互式等距科学图 | `npx skills add Garinmckayl/anima -g -a claude-code` |

## 通用前置

- Claude Code 或其他 Agent Skills host（Codex、OpenCode、Antigravity 等）。
- 多数技能要求 Node.js 20+；具体版本见各技能页。
- 部分技能额外需要：`ffmpeg`（视频）、Python 3（声音）、Chromium/Playwright（截图/录制）。
- 通用安装模式：`npx skills add <owner>/<repo> -g -a claude-code`；插件型技能用 `/plugin marketplace add` + `/plugin install`。

## 说明

- 这些都是第三方技能/工具，不是本项目维护的代码；使用前请阅读上游 LICENSE 和 README。
- 安装命令和用法按各上游 README（2026-11-14）整理；上游可能变化，以仓库/官网为准。
- 本仓库只做整理和索引，不包含这些技能的源码，也不对其安全性、生成内容的准确性作保证。
