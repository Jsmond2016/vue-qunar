## 工程启动流程

``` bash
# 切换到课程章节对应的分支上（重要！）
git checkout 分支名

# 安装项目依赖
npm install

# 启动开发环境服务器
npm run dev
```

- 遇到问题

 如果 启动后拿不到数据，可能需要根据 /config/index.js 启动一个后端服务
 
 ```js
 proxyTable: {
      '/api': {
        target: 'http://localhost:8080',
        pathRewrite: {
          '^/api': '/static/mock'
        }
      }
 
 ```
