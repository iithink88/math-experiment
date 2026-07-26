# math-experiment · 数学实验技能

把数学问题变成**可交互的 2D / 3D 实验**：拖动滑块、旋转视角、实时看规律。
基于 Plotly.js（2D）与 Three.js（3D），纯前端、零本地依赖、零密钥，浏览器直接打开即用。

## 功能

- **2D 实验**：函数性质探索（二次 / 三角 / 指数）、统计分析、平面几何、微积分可视化
- **3D 实验**：3D 函数曲面、空间几何体、3D 曲线、旋转体与曲面、3D 向量
- 参数滑块实时驱动图形；变换路径追踪；亮色 / 暗色主题切换；自动旋转动画
- 确认流程：先出实验方案，用户确认后再生成 HTML，避免直接造轮子

## 安装（3 种方式）

1. **最省事**：把本仓库的 `SKILL.md` 直接拖进 WorkBuddy 聊天框，按提示安装
2. **手动**：把整个仓库文件夹放进 `~/.workbuddy/skills/math-experiment/`
   （Windows 路径：`C:\Users\<你>\.workbuddy\skills\math-experiment\`）
3. **命令行**：`npx skills add iithink88/math-experiment@math-experiment`

## 目录结构

```
math-experiment/
├── SKILL.md                          # 技能定义（AI 执行指令）
├── assets/
│   ├── math-experiment-template.html   # 2D 模板（Plotly.js）
│   └── math-experiment-3d-template.html # 3D 模板（Three.js）
├── demo/                             # 成品例子展示
│   ├── 一元一次函数图像实验.html        # 一元一次函数 y=kx+b 图像探索
│   └── cone_projection_area.html       # 圆锥侧面积验证（投影法）
├── LICENSE
└── .gitignore
```

## 在线 Demo

- 一元一次函数：`https://iithink88.github.io/math-experiment/demo/%E4%B8%80%E5%85%83%E4%B8%80%E6%AC%A1%E5%87%BD%E6%95%B0%E5%9B%BE%E5%83%8F%E5%AE%9E%E9%AA%8C.html`
- 圆锥侧面积（投影法）：`https://iithink88.github.io/math-experiment/demo/cone_projection_area.html`

> 球面构建自 Three.js CDN，首次打开需联网加载库文件。

## 使用示例

在 WorkBuddy 中直接说：

- "用 math-experiment 做一个二次函数顶点随 a 变化的实验"
- "用 math-experiment 验证圆锥侧面积"
- "用 math-experiment 画出正弦函数的振幅和频率"

技能会先给出实验方案（参数、范围、观察点），你确认后生成可交互 HTML。

## 许可

MIT —— 自由使用、修改、再分发。
