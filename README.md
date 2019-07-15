# node-babel7-es6

### 1. 安装依赖
```
npm i --save-dev @babel/core @babel/register @babel/plugin-proposal-class-properties @babel/plugin-transform-async-to-generator @babel/plugin-transform-modules-commonjs
```
### 2. 配置.babelrc文件

```javascript
{
    "plugins": [
      "@babel/plugin-transform-async-to-generator",
      "@babel/plugin-transform-modules-commonjs",
      "@babel/plugin-proposal-class-properties"
    ]
}
```

### 3. 写入口文件index.js
```
require('@babel/register');
require('../app') // 要运行的文件
```

### 4. 启动
```
node index.js
```