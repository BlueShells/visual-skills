# factory-skill

**微缩 3D 工厂流水线场景动画。**

- 来源：https://github.com/AirsupHQ/factory-skill
- 许可：MIT
- 适合：产线规划、产能演示、瓶颈分析、教学。

## 它做什么

用一句话描述工厂，Claude 生成一个**单文件 HTML**：倾斜移轴镜头下的微缩工厂，机器在运转、产品在传送带上流动；底层是真实的离散事件仿真（工位、节拍、批次、有限缓冲、班次、故障、报废）。HUD 实时显示：

- 吞吐 vs 目标
- takt、WIP、lead time
- 每个工位的 busy/blocked/starved/down
- 红色脉冲标出的瓶颈

点击工位可以加机器、改节拍或缓冲，观察瓶颈移动。

## 安装

```sh
npx skills add AirsupHQ/factory-skill -g -a claude-code
```

要求：Node.js 20+；零依赖，不需要 `npm install`，也不需要 API key。

## 用法

在 Claude Code 中：

```text
/factory a line that makes 2,000 e-bike motors a day
```

其他例子：

```text
/factory a bakery that bakes 10,000 croissants an hour
/factory a 4 GWh battery cell gigafactory, coating to formation, three shifts
```

## 产出

- 一个自包含 HTML 页面，浏览器直接打开。
- 页面内可交互调整工位参数，瓶颈和指标实时重算。
- 仓库内提供示例 HTML 画廊。
