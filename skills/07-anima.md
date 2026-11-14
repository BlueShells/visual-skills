# anima

**适合理化实验、教学科普演示。**

- 来源：https://github.com/Garinmckayl/anima
- 许可：MIT
- 适合：生物、神经科学、药理学机制图；也包含分子/化学结构绘制工具。

## 它做什么

把一句生物学/科学描述变成可交互、带引用的等距科学图：真实结构、可切换的机制、由小模型驱动的读数，屏幕上的每个数字都有来源和条件。它区分“已确立的结论”“某一主流模型”“啮齿动物证据”“人类证据”，不能验证的数字会省略；明确教育用途，不给剂量/用法建议。

## 安装

```sh
npx skills add Garinmckayl/anima -g -a claude-code
```

要求：Claude Code + Node.js ≥ 20.10；零运行时依赖；Chrome/Chromium 只在截图/验证脚本时需要。

## 用法

```text
/anima show how cocaine and amphetamine act differently at the dopamine transporter, with a drug selector and sourced mechanisms; standalone HTML
```

```text
/anima visualize semaglutide acting on a pancreatic beta cell, with glucose-dependent insulin release, cited label numbers and an educational-use note
```

```text
/anima show D1 and D2 receptor signalling in a striatal neuron, with the G-protein cycle and a receptor-antagonist toggle
```

## 产出

- 独立 HTML，暗/亮主题，SVG（可选 WebGL/3D）。
- 图内可切换机制/抑制剂/浓度等；每个数字带引用。
- 规模分级：Figure（40–80 零件，约 30–90 分钟）、Hero（80–150 零件，2–4 小时）、Epic（6 小时以上，需用户确认）。
- 定位是教学/科普，不是医学建议。
