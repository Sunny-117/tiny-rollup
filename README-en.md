# tiny-rollup [![npm](https://img.shields.io/npm/v/tiny-rollup.svg)](https://npmjs.com/package/tiny-rollup)

English | <a href="./README-zh_CN.md">简体中文</a>

<img src="./assets/logo.webp" width="100%">

tiny-rollup is a lightweight and efficient JavaScript bundler designed for rapid construction and packaging of modern web applications. With its simple yet powerful workflow, tiny-rollup is dedicated to providing optimal performance and development experience.

## Features

📦️ Lightweight: tiny-rollup focuses on minimizing the size of the bundling tool, ensuring fast startup and loading times.

🔧 Simple Configuration: Provides concise and intuitive configuration options, allowing for easy customization and adjustment of the project's bundling process.

🔥 Tree-shaking: Automatically removes unused code through static analysis, reducing the size of the final bundled file.

## Install

```bash
pnpm i tiny-rolluptiny-rollup
```

## Usage

```ts
import { dirname, resolve } from 'node:path'
import { fileURLToPath } from 'node:url'
import { tiny-rollup } from 'tiny-rolluptiny-rollup

const __filename = fileURLToPath(import.meta.url)
const __dirname = dirname(__filename)

const entry = resolve(__dirname, './msg.js')
tiny-rollup(entry, resolve(__dirname, '../bundle.js'))
```

See an [example](https://github.com/Sunny-117/tiny-rollup/blob/main/playground/src/index.js) for more details.

## License

[MIT](./LICENSE) License © 2024 [Sunny-117](https://github.com/sunny-117)
