# vrux


想必很多人和我一样，同时有着Vue和React的开发经验，同时也在Vue中普遍使用vuex，在React、React Native使用redux。
做了之后，你会发现，其实他们的代码结构是很类似的，具体可以参考我做的两个脚手架项目：

- [vue-vuex](https://github.com/okoala/vue-vuex)
- [react-redux-antd](https://github.com/okoala/react-redux-antd)

那应该是可以合在一起的，不管你在微信端用Vue，还是写React Native，在或者在其他地方用React + Ant.Design所有的业务代码，数据state 都可以统一起来。项目可以是类似下面的目录架构：

```
  AwesomeProject
      --- build
      --- config
      --- server
      --- src
            --- assets (公用资源)
            --- vrux
                  --- api (接口)
                  --- constants (常量)
                  --- modules (业务逻辑模块)
                        --- global
                        --- account
                        --- user
                        --- comment
                  --- middlewares (中间件)
                  --- util
                  --- test (测试)
            --- weixin (vue) 
                  --- components (组件)
                  --- route.js (路由)
                  --- views (视图)
                  --- test (测试)
            --- pc (react＋ant.design)
                  --- components (组件)
                  --- route.js (路由)
                  --- views (视图)
                  --- test (测试)
            --- mobile (react native)
                  --- components (组件)
                  --- route.js (路由)
                  --- views (视图)
                  --- test (测试)
      --- package.json
```

暂时就这么定下了~~
