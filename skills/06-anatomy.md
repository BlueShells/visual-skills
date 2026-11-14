# anatomy

**线稿风，可做机械运转、零件拆解。**

- 来源：https://github.com/wheresryan22/anatomy
- 许可：MIT
- 适合：技术概念、机械结构、运转原理、零件拆解；也可用于把抽象概念变成“会动的实物”。

## 它做什么

让 Claude 为一个技术概念发明一个“工作原理就是该概念”的物理对象，然后用几十个精细零件把它搭出来：等距视角、线稿/实体着色、带标题和实时读数，鼠标和键盘可以驱动；每个数字都来自驱动零件运动的同一个小模型。输出 SVG，可选 WebGL/3D。

## 安装

```sh
npx skills add wheresryan22/anatomy -g
```

CLI 会问你给哪些 agent 安装（Claude Code、Antigravity、OpenCode、Codex、MiniMax Code）；跳过问答加 `-a claude-code` 等。要求 Node.js ≥ 20.10；零依赖。

## 用法

```text
/anatomy explain how a token bucket rate limiter works, interactive
```

其他例子：

```text
/anatomy show how a pin-tumbler lock opens when every pin matches
/anatomy explain a GPU context serving many canvases as a gantry plotter visiting 16 wells
```

在 Codex 中用 `$anatomy`；Antigravity/OpenCode/MiniMax Code 用 `/anatomy`。

## 产出

- 等距 SVG/WebGL/3D 图，带标题、提示和实时读数。
- 零件数量按规模分级（Figure/Hero/Epic），Epic 需要用户确认。
- 自带缩放检查，确保每个关节都对得上。
