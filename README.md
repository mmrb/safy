# 纯前端自动化测试系统

### 环境

- MySQL
- Node.js

### 获取代码：
    git clone https://github.com/mmrb/safy.git

### 运行
    cd safy
    npm install
    node index.js

### 使用

服务默认在3000端口启动，用浏览器打开[http://localhost:3000](http://localhost:3000)；

程序首先会检测`app/setting.js`配置文件是否存在，如果不存在，则会重定向到初始化界面[http://localhost:3000/initsafy](http://localhost:3000/initsafy)，填写MySQL配置、网站访问路径和端口配置；最后程序生成的`app/setting.js`文件内容大致如下：

```javascript
module.exports = {
    "mysql" : {
        "host" : "localhost",
        "user" : "root",
        "password" : "password",
        "database" : "safy"
    },
    "site" : {
        "domain" : "localhost:3000",
        "port" : "3000"
    }
}
```

回到登录界面，注册帐号，登录进入系统，Enjoy it！
