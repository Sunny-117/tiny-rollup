# tiny-rollup [![npm](https://img.shields.io/npm/v/tiny-rollup.svg)](https://npmjs.com/package/tiny-rollup)

[![npm version][npm-version-src]][npm-version-href]
[![npm downloads][npm-downloads-src]][npm-downloads-href]
[![bundle][bundle-src]][bundle-href]
[![JSDocs][jsdocs-src]][jsdocs-href]
[![License][license-src]][license-href]

简体中文 | <a href="./README-en.md">English</a>

<img src="./assets/logo.webp" width="100%">

tiny-rollup 是一个轻量级且高效的 JavaScript 打包工具，专为现代 Web 应用的快速构建和打包而设计。通过简单而强大的工作流程，致力于提供最佳的性能和开发体验。

## 特性

📦️ 轻量级：tiny-rollup 注重最小化打包工具的体积，确保快速启动和加载时间。

🔧 简单配置：提供简洁直观的配置选项，轻松自定义和调整项目的打包过程。

🔥 tree-shaking：通过静态分析代码，自动移除未使用的代码，减小最终打包文件的大小。

## 安装

```bash
pnpm i tiny-rollup
```

## 使用

```ts
import { dirname, resolve } from 'node:path'
import { fileURLToPath } from 'node:url'
import { tinyRollup } from 'tiny-rollup'

const __filename = fileURLToPath(import.meta.url)
const __dirname = dirname(__filename)

const entryTest1 = resolve(__dirname, './main.js')
const outTest1 = resolve(__dirname, '../dist/bundle.js')

tinyRollup(entryTest1, outTest1)
```

查看[示例](https://github.com/Sunny-117/tiny-rollup/blob/main/playground/src/index.js)了解更多详情。

## License

[MIT](./LICENSE) License © [Sunny-117](https://github.com/Sunny-117)

<!-- Badges -->

[npm-version-src]: https://img.shields.io/npm/v/tiny-rollup?style=flat&colorA=080f12&colorB=1fa669
[npm-version-href]: https://npmjs.com/package/tiny-rollup
[npm-downloads-src]: https://img.shields.io/npm/dm/tiny-rollup?style=flat&colorA=080f12&colorB=1fa669
[npm-downloads-href]: https://npmjs.com/package/tiny-rollup
[bundle-src]: https://img.shields.io/bundlephobia/minzip/tiny-rollup?style=flat&colorA=080f12&colorB=1fa669&label=minzip
[bundle-href]: https://bundlephobia.com/result?p=tiny-rollup
[license-src]: https://img.shields.io/github/license/Sunny-117/tiny-rollup.svg?style=flat&colorA=080f12&colorB=1fa669
[license-href]: https://github.com/Sunny-117/tiny-rollup/blob/main/LICENSE
[jsdocs-src]: https://img.shields.io/badge/jsdocs-reference-080f12?style=flat&colorA=080f12&colorB=1fa669
[jsdocs-href]: https://www.jsdocs.io/package/tiny-rollup
