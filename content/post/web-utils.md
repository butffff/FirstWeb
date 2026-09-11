---
title: WebUtils 前端工具集介绍
categories: ["projects"]
tags: ["Projects","WebUtils","Frontend"]
cover: /images/covers/post/webutils/cover.png
description: WebUtils 是一个自用的高质量前端代码合集，包含动态文本特效引擎等模块，纯原生实现，零依赖，配置灵活，MIT 开源。
banner: /images/covers/post/webutils/cover.png
date: 2026-09-02T03:00:00+08:00
lastmod: 2026-09-02T03:00:00+08:00
---

## 仓库简介

[WebUtils](https://github.com/CrimsonSeraph/WebUtils) 是我在日常前端开发中积累的可复用代码片段仓库。每个模块都力求：

- **功能独立** – 不依赖第三方库，纯原生 HTML/CSS/JS 实现
- **配置灵活** – 通过 `data-*` 属性或 CSS 变量控制行为
- **易于移植** – 单个 `.html` + `.css` + `.js` 文件，拷贝即用

所有代码均采用 **MIT 许可证** 开源，可自由用于个人或商业项目，仅需保留原始版权声明。

> 🧪 在线演示：<https://#>（待补充）

## 模块列表

### 1. 动态文本特效引擎（DynamicTextEngine）

一个为网页文字添加丰富动态效果的轻量级引擎，支持以下特性（无需 CSS 支持）：

- **单色文本**：预设语义色（警告/成功/错误）或任意自定义颜色
- **多色文本**：一行文字内不同片段独立着色
- **渐变变色**：平滑循环过渡，可自定义色值序列与动画时长
- **抖动文本**：整体抖动或每个字符独立抖动，支持 6 档速度调节
- **乱码引擎**：将真实文本替换为随机符号，支持自定义字符集，并可通过父级属性“无效化”恢复原文
- **文本方向切换与片段轮播**：主体文字逐个字符消失，额外片段逐个字符出现，支持方向控制、顺序/随机、切换次数限制、动画速度调节

> 🔗 演示地址：<https://#>（待补充）
> 📂 源码目录：[WebUtils/DynamicTextEngine/](https://github.com/CrimsonSeraph/WebUtils/tree/main/DynamicTextEngine)

- **第一部分**
![DynamicTextEngine](/images/covers/post/webutils/DynamicTextEngine_1.png)

- **第二部分**
![DynamicTextEngine](/images/covers/post/webutils/DynamicTextEngine_2.png)

## 使用方式

1. 克隆或下载本仓库。
2. 复制需要的模块文件夹到你的项目中。
3. 在 HTML 中引入 CSS 和 JS 文件，按示例添加标记即可生效。

例如使用动态文本特效：

```html
<link rel="stylesheet" href="DynamicTextEngine.css">
<script src="DynamicTextEngine.js"></script>

<div class="effect-text mono-color" data-type="warning">磁盘空间不足</div>
```

更详细的配置属性请参考模块内的 `README.md`。

## 后续计划

- 添加按钮特效组件（悬停动画、点击波纹、加载状态等）
- 表单美化模块（自定义复选框、滑块、输入框）
- 纯 CSS 加载动画集合
- 常用工具函数库（节流、防抖、深拷贝等）

欢迎通过 [Issue](https://github.com/CrimsonSeraph/WebUtils/issues) 提出需求或贡献代码。

## 许可证

MIT © 2026 CrimsonSeraph(ltyy.leoyu@gmail.com)
