# vue-start
[![wechat-group](https://badgen.net/badge/wechat/wechat)](http://ganquanzhong.top)
[![ForFuture](https://badgen.net/badge/ForFuture/gqzdev/cyan)](http://ganquanzhong.top)
[![github](https://badgen.net/badge/github/github?icon)](https://github.com/gqzdev)
[![csdn](https://badgen.net/badge/blog/ganquanzhong/red)](https://blog.csdn.net/ganquanzhong)
[![stars](https://badgen.net/github/stars/gqzdev/vue-start)](https://github.com/gqzdev/shop)
[![forks](https://badgen.net/github/forks/gqzdev/vue-start)](https://github.com/gqzdev/shop)
[![last-commit](https://badgen.net/github/last-commit/gqzdev/vue-start)](https://github.com/gqzdev/shop)
[![prs](https://badgen.net/github/prs/gqzdev/vue-start)](https://github.com/gqzdev/shop)
[![gitee](https://badgen.net/badge/gitee/zhong96/orange)](https://gitee.com/zhong96)

# 这在里发布关于Vue开发的案例和技术原理讲解

## 说明
|   |   |
|--|--|
|[VueTest](https://github.com/gqzdev/vue-start/tree/master/VueTest) | 入门vue的语法知识|
|[Vuedemo](https://github.com/gqzdev/vue-start/tree/master/VueDemo) | 入门vue项目开发的一些案例|
|[VuexTest](https://github.com/gqzdev/vue-start/tree/master/VuexTest) | vuex的状态管理案例|
|[VueSource](https://github.com/gqzdev/vue-start/tree/master/VueSource) | vue的部分源码分析|




## vuedemo项目中包含多个案例
   使用npm install --save '需要的依赖'
   配置当前项目是运行那一个 
   在VueDemo\build\webpack.base.conf.js文件中修改
   ```javascript
         /*指定app主应用src*/
      module.exports = {
        context: path.resolve(__dirname, '../'),
        entry: {
          //修改src_模块即可
          app: './src_mint-ui/main.js'
        },
        output: {
          path: config.build.assetsRoot,
          filename: '[name].js',
          publicPath: process.env.NODE_ENV === 'production'
            ? config.build.assetsPublicPath
            : config.dev.assetsPublicPath
        },
  
    
    
