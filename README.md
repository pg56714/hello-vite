# hello-vite

## Getting Started

build tools: vite
Vite is a modern frontend development tool that offers fast startup, instant hot reload, and optimized production builds.

```bash
npm create vite@latest
```

```bash
npm i
```

```bash
npm run dev
```

```bash
npm run build
```

build --> generate dist folder

The two important aspects of bundling are:

1. code minification：Compresses code to reduce file size and improve loading speed.
2. tree shaking：Removes unused code to optimize application performance.

## Additional

Common usage: putting all the code into a single file.

Settings：vite.config.js

```bash
npm install vite-plugin-singlefile --save-dev
```

```js
import { defineConfig } from "vite";
import { viteSingleFile } from "vite-plugin-singlefile";

export default defineConfig({
  plugins: [viteSingleFile()],
});
```

```bash
npm run build
```

## Source

[vite-introduce](https://www.youtube.com/watch?v=vj8KSZjPTUU)
