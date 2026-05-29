# 模块

Node.js 既支持 ES 模块也支持 CJS 模块，但每个文件的格式由其文件扩展名以及在文件所在目录及其所有祖先目录中找到的第一个 package.json 文件的 type 字段决定：

- .mjs 和 .cjs 文件分别始终被解释为 ES 模块和 CJS 模块。

- 如果最近的 package.json 文件包含值为 "module" 的 type 字段，则 .js 文件会被解释为 ES 模块。如果没有 package.json 文件，或者 type 字段缺失或具有任何其他值， .js 文件会被解释为 CJS 模块。