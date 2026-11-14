# machine-skill

**重型机械演示，支持高拟真可交互 3D 网页。**

- 来源：https://github.com/AirsupHQ/machine-skill
- 许可：MIT
- 适合：航空发动机、火箭发动机、泵、机械表、LVAD 等复杂机械的原理与结构演示。

## 它做什么

用一句话描述机器，Claude 研究会研究真实尺寸和物理，生成**单文件 HTML**：真实比例的 PBR 材质、棚拍灯光、由小型求解器驱动的运动部件（推力、扭矩、转速、流量、压力、效率）。支持：

- explode（爆炸视图）
- cutaway（剖切，剖面有实体封盖）
- x-ray
- slow-mo
- labels
- break it（破坏）
- 一键录制 20–30 秒成片

## 安装

```sh
npx skills add AirsupHQ/machine-skill -g -a claude-code
```

要求：Node.js 20+；Three.js 0.170 随技能打包，无构建步骤。

## 用法

```text
/machine a turbofan jet engine, the kind that pushes a widebody off the runway
```

```text
/machine a mechanical watch movement, the escapement ticking
```

录制视频：

```sh
node ~/.claude/skills/machine/scripts/record.mjs watch.html out/watch.mp4 --music freepd:Classical/Easy_Lemon
```

## 产出

- 一个可打开、可拖动、可剖切、可爆炸的 HTML 3D 仿真。
- 屏幕上的数值由求解器计算，不是预先写死的表。
- 可选 MP4 成片，用于演示或发布。
