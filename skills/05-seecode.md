# SeeCode

**流程演示动画，适合硬件、流程可视化。**

- 来源：https://github.com/Aryanutkarsh/SeeCode
- 许可：MIT
- 适合：架构图、流程图、时序图、ER、甘特、桑基、3D 等距图等。

## 它做什么

把一段简短的 JSON/自然语言 spec 变成编辑级、可动画、可探索的图：一个 HTML 文件，可以悬停追踪、点击、逐步讲解；也可以导出 SVG、PNG、GIF、MP4。支持 45 种图类型，零依赖。

## 安装

**Claude Code 插件（推荐，跟随最新版）：**

```text
/plugin marketplace add Aryanutkarsh/seecode
/plugin install seecode@seecode
```

**Cursor、Codex、OpenCode 等：**

```sh
npx skills add Aryanutkarsh/seecode -g
```

要求：Node.js 20+；零 npm 依赖。

## 用法

```text
Use SeeCode to show how checkout works: the browser calls the API,
the API writes to Postgres, charges Stripe and publishes an event to Kafka.
```

继续用自然语言调整：

> highlight the payment path

> make it dark

> export it for my slides

## 产出

- 单文件 HTML，可交互、可逐步播放。
- 可导出 SVG/PNG/GIF/MP4。
- 支持主题和品牌色；可导入已有图表。
