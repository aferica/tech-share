快速搭建自己的API服务器和网站

---



1.Node服务器搭建

使用Node + Express + Mongodb快速搭建API服务器

---



1.1 项目简单目录结构介绍
```

.		#项目总目录
├── config    #项目配置文件夹
│   ├── db_config.js    #数据库配置文件
├── models    #逻辑模块文件夹
│   ├── user    #user模块文件夹
│   │   ├── user_controller.js    #user逻辑实现文件
│   │   ├── user_model.js   #user模型文件
|
├── route.js    #程序路由文件夹
│   ├── user_route.js   #user模块路由文件
|
├── app.js    #程序入口文件
└── package.json#Node项目依赖文件
```
---

1.2 项目基本配置介绍



    const express = require("express"); 
    const path = require("path"); 
    const bodyParser = require("body-parser"); 
    const compress = require('compression'); 
    const logger = require('morgan'); 
    const crypto = require("crypto"); 
    const mongoose = require('mongoose'); 
    const session = require('express-session'); 
    const MongoStore = require('connect-mongo')(session); 
    const moment = require('moment'); 
    const dbURI = require('./config/db_connection').dbURI;
    mongoose.createConnection(dbURI); //连接数据库

---



2.Angular2网站快速实现

---



3.服务器Nginx部署

---



4.常用工具推荐

---


