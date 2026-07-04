# @vvi/rollup-preserve-directive

[![version](<https://img.shields.io/npm/v/@vvi/rollup-preserve-directive.svg?logo=npm&logoColor=rgb(0,0,0)&label=版本号&labelColor=rgb(73,73,228)&color=rgb(0,0,0)>)](https://www.npmjs.com/package/@vvi/rollup-preserve-directive) [![issues 提交](<https://img.shields.io/badge/issues-提交-rgb(255,0,63)?logo=github>)](https://github.com/MrMudBean/rollup-preserve-directive/issues)
  
在使用 rollup 打包时保留 `"use client/server";` 指令而不报错。

## 安装

```bash
npm install --save-dev @vvi/rollup-preserve-directive
```

## 使用

作为 rollup 的第一个插件即可：

```js
import { preserveDirective } from '@vvi/rollup-preserve-directive';

export default {
  // ... 其他配置

  plugins: [
    preserveDirective(), // 保留 `use client/server` 指令且不报错

    // ... 其他插件
  ],

  // ... 其他配置
};
```
