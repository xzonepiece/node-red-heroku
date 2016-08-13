
node-red-heroku
================

将[Node-RED](http://nodered.org) 部署到[Heroku](https://www.heroku.com)。

### 信用卡用户请直接点击下面的按钮自动安装
[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/joeartsea/node-red-heroku)

### 无信用卡的免费账户
1. app.json文件中不能填写任何插件；
2. 在[mLab](https://mlab.com/)网站上获取免费账号，并建立数据库，获得MongoDB URI地址，填入setting.js文件中；
3. 不能安装“node-red-node-mongodb”，即不能在packages.json文件中不能填入“node-red-node-mongodb”，否则在使用中会造成“Error:node not deployed”错误。

### 设置密码
默认情况下，任何人都可以登录网站的编辑界面，并且可以修改flows，为了防止其他人进入，可输入以下命令，设置密码：
* heroku config:set NODE_RED_USERNAME = the username to secure the editor with
* heroku config:set NODE_RED_PASSWORD = the password to secure the editor with
