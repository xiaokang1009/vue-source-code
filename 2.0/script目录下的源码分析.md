# `script`目录
`vue.js`中`script`目录包含打包vue相关的配置文件,主要包含下面的几个文件
##  `alias.js`
```javascript
    // 配置路径别名
    const path = require('path') // 引入node中path类库

    const resolve = p => path.resolve(__dirname, '../', p) 

    module.exports = {
        vue: resolve('src/platforms/web/entry-runtime-with-compiler'),
        compiler: resolve('src/compiler'), 
        core: resolve('src/core'), 
        shared: resolve('src/shared'), 
        web: resolve('src/platforms/web'),
        weex: resolve('src/platforms/weex'),
        server: resolve('src/server'),
        sfc: resolve('src/sfc')
    }
```
## `build.js`

