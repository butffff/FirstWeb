---
title: Introduction to WebUtils Frontend Toolkit
categories: ["projects"]
tags: ["Projects","WebUtils","Frontend"]
cover: /images/covers/post/webutils/cover.png
description: WebUtils is a collection of high-quality, reusable front-end code snippets, including a dynamic text effects engine, pure native implementation, zero dependencies, flexible configuration, MIT licensed.
banner: /images/covers/post/webutils/cover.png
date: 2026-05-28T03:00:00+08:00
lastmod: 2026-05-28T03:00:00+08:00
---

## Overview

[WebUtils](https://github.com/CrimsonSeraph/WebUtils) is my personal collection of reusable front-end code snippets accumulated during daily development. Each module strives to be:

- **Standalone** – pure HTML/CSS/JS, no third-party libraries
- **Flexible** – behavior controlled via `data-*` attributes or CSS variables
- **Portable** – single `.html` + `.css` + `.js` files, copy and use

All code is open-sourced under the **MIT License**, free for personal or commercial use, with the only requirement to retain the original copyright notice.

> 🧪 Live Demo: <https://#> (to be added)

## Modules

### 1. Dynamic Text Effects Engine (DynamicTextEngine)

A lightweight engine that adds rich dynamic effects to web text, featuring (No CSS support required ):

- **Mono Color Text**: preset semantic colors (warning/success/error) or any custom color
- **Multi-Color Text**: independent coloring for different segments within one line
- **Gradient Color Change**: smooth cyclic transitions, customizable color sequences and duration
- **Shaking Text**: global shake or per-character independent shake, with 6 speed levels
- **Obfuscation Engine**: replaces real text with random symbols, supports custom character sets, and can be "deobfuscated" via parent attribute to restore original text
- **Text Direction Switching & Carousel**: original text disappears character by character, then extra fragments appear character by character, supports direction control, sequential/random order, switch count limit, animation speed adjustment

> 🔗 Demo URL: <https://#> (to be added)
> 📂 Source directory: [WebUtils/DynamicTextEngine/](https://github.com/CrimsonSeraph/WebUtils/tree/main/DynamicTextEngine)

- **First Part**
![DynamicTextEngine](/images/covers/post/webutils/DynamicTextEngine_1.png)

- **Second Part**
![DynamicTextEngine](/images/covers/post/webutils/DynamicTextEngine_2.png)


## Usage

1. Clone or download this repository.
2. Copy the desired module folder into your project.
3. Include the CSS and JS files in your HTML, and add the required markup as shown in examples.

Example using the dynamic text effect:

```html
<link rel="stylesheet" href="DynamicTextEngine.css">
<script src="DynamicTextEngine.js"></script>

<div class="effect-text mono-color" data-type="warning">Low disk space</div>
```

Refer to the `README.md` inside each module for detailed configuration options.

## Roadmap

- Button effect components (hover animations, ripple, loading states)
- Form styling modules (custom checkboxes, sliders, inputs)
- Pure CSS loading animations collection
- Utility function library (throttle, debounce, deep clone, etc.)

Feel free to submit feature requests or contributions via [Issues](https://github.com/CrimsonSeraph/WebUtils/issues).

## License

MIT © 2026 CrimsonSeraph(ltyy.leoyu@gmail.com)