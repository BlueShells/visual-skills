# teardown

**3D 可交互机械动画，可做大型/仿生机械拆解。**

- 来源：https://github.com/elvarofficial/teardown
- 许可：MIT
- 适合：发动机、机械臂、仿生机器人、任何“想拆开看内部”的机器。

## 它做什么

用一句话描述一台机器，Claude 生成一个**离线单文件 HTML**：Three.js 机器在中间运行，周围面板显示真实数值，按钮可以拆开正在工作的部件；无人操作时页面会自己巡览。还可以逐帧渲染 60fps MP4，并生成程序化音效。

## 安装

```sh
npx skills add elvarofficial/teardown -g -a claude-code
```

安装后在技能目录里执行一次：

```sh
npm install && npx playwright install chromium
```

要求：Node.js 20+；录制视频需要 `ffmpeg`；生成声音需要 Python 3。

## 用法

直接用自然语言：

> Build me a simulator of a 4-stroke motorcycle engine I can take apart.

> How does a mechanical watch keep time? Show me as a simulator.

> Make a teardown of a hydraulic excavator arm and record a 20-second video of it.

也可以先跑自带示例：

```sh
node sims/build.mjs v8-live
node sims/build.mjs cessna-live
node sims/build.mjs strandbeest-live
```

## 产出

- `teardown-out/dist/<name>.html`：单文件、离线可打开的 3D 拆解页面。
- 可选 60fps MP4 和程序化音效。
- 内置 3 个完整示例：V8 发动机、Cessna 337、Strandbeest SB-10。
