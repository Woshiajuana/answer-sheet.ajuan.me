这在 JavaScript 文件的 JSDoc 注释中尤其有用，因为否则无法导入类型：

```js
/** @type {import("webpack").Configuration} */
module.exports = {
  // ...
}
```