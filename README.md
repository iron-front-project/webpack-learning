# 前端模块化
## CommonJS
**核心思想:**通过require方式来同步加载依赖的其他模块，通过module.exports导出需要暴露的接口。
**应用：**Node.js采用这种方式，后推广到网页开发。
**举例：**
	`const moduleA = require('./moduleA');`
	`module.exports = moduleA.someFunc;`
**优点：**
（1）代码可以复用于Node.js环境并运行，可以做应用同构；
（2）npm发布的第三方模块都采用了CommonJS规范
**缺点：**代码无法直接运行在浏览器环境下，必须通过工具转换成标准的ES5

