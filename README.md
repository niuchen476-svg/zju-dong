# 智能交互台灯 - 技术与设计方案

## 1. 项目愿景
本项目旨在通过 **计算设计 (Computational Design)** 理念，解决传统照明设备与人交互生硬的问题。

## 2. 核心数学模型
本 Demo 模拟了光流感应逻辑。当用户距离传感器 $d$ 发生变化时，系统通过以下公式计算亮度 $L$：

$$
L(d) = 
\begin{cases} 
100\% & d < 30 \\ 
100 \cdot e^{-k(d-30)} & d \ge 30 
\end{cases}
$$

> **设计推导：** 使用指数衰减函数，确保灯光熄灭时具有“呼吸感”，提升情感交互体验。

## 3. 技术栈实现
- **前端架构：** HTML5 + CSS3 (Apple Design Style)
- **交互逻辑：** JavaScript (模拟异步 API 调用)
- **文档规范：** Markdown + LaTeX 数学公式

## 4. 如何运行
1. 使用 **VS Code** 打开本项目。
2. 点击右下角 `Go Live` 按钮。
3. 点击网页中的“开始诊断”查看 AI 模拟反馈。
  <script src="https://polyfill.io/v3/polyfill.min.id?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$']]
    }
  };
</script>
