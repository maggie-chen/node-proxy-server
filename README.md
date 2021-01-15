# node-proxy-server
简单易用的node本地代理服务器

## 使用方法
* 将server.js拷贝到你的项目根目录
* 修改js文件中的config配置

```
let conifg = {
    '/xxxx': { // 需要拦截的本地请求路径
        target: 'http://xxxxxxxx.com', // 真实代理地址
        port: 80, // 端口，默认80
    }
    // ...other path （支持多路径拦截）
};
```
* 启动服务 `node serve.js`（本地端口暂定 8000，可在js文件中定制）
```
app.listen(你的端口号);
```

* 打开浏览器，访问你的项目路径，例如：http://localhost:8000/index.html

## 依赖项
* node （请确保你的系统安装有node）