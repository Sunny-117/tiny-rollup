# tiny-rollup [![npm](https://img.shields.io/npm/v/tiny-rollup.svg)](https://npmjs.com/package/tiny-rollup)

简体中文 | <a href="./README-en.md">English</a>

<img src="./assets/logo.webp" width="100%">

tiny-rollup 是一个轻量级且高效的 JavaScript 打包工具，专为现代 Web 应用的快速构建和打包而设计。通过简单而强大的工作流程，致力于提供最佳的性能和开发体验。

## 特性

📦️ 轻量级：tiny-rollup 注重最小化打包工具的体积，确保快速启动和加载时间。

🔧 简单配置：提供简洁直观的配置选项，轻松自定义和调整项目的打包过程。

🔥 tree-shaking：通过静态分析代码，自动移除未使用的代码，减小最终打包文件的大小。

## 安装

```bash
pnpm i tiny-rolluptiny-rollup
```

## 使用

```ts
import { dirname, resolve } from 'node:path'
import { fileURLToPath } from 'node:url'
import { tiny-rollup } from 'tiny-rolluptiny-rollup

const __filename = fileURLToPath(import.meta.url)
const __dirname = dirname(__filename)

const entry = resolve(__dirname, './msg.js')
tiny-rollup(entry, resolve(__dirname, '../bundle.js'))
```

查看[示例](https://github.com/Sunny-117/tiny-rollup/blob/main/playground/src/index.js)了解更多详情。

## 开源协议

[MIT](./LICENSE) License © 2024 [Sunny-117](https://github.com/sunny-117)
