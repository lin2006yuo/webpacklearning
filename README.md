# webpacklearning
webpack学习项目

*分模块打包，将公共包和逻辑代码分离
```
    config.entry = {
        app: path.join(__dirname, 'src/index.js'),
        vendor: ['vue']
    }
    
    config.plugins.push(
        new webpack.optimize.CommonsChunkPlugins({
            name: 'vendor'
        })
    )
```
