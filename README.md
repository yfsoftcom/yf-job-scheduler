## yf-job-scheduler
> 可以通过web来创建定时任务，定时执行，记录执行结果

### 0.Overview
* 任务列表界面：
![任务列表](http://upload-images.jianshu.io/upload_images/1449977-ea0f7c1ffed50831.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 创建任务界面：
![创建任务](http://upload-images.jianshu.io/upload_images/1449977-fda0dc1a72b2cf38.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

源码奉上: [https://github.com/yfsoftcom/yf-job-scheduler](https://github.com/yfsoftcom/yf-job-scheduler),欢迎拍砖

前提是你要有一些cron表达式的基础哦~

### 1. Install
```
$ git clone https://github.com/yfsoftcom/yf-job-scheduler.git

$ cd yf-job-scheduler

$ npm install
```
### 2. Config
```
$ cp key_default.js key.js

$ vi key.js
```

填写appkey 和 secretkey

这个是在yf-api-server中生成的key

### 3. Run
```
$ npm start
//或者使用pm2来启动
$ pm2 start bin/www -i 1 --name yf-job-scheduler
```
打开浏览器：[http://localhost:3000](http://localhost:3000)

Enjoy It~
