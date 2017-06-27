====
简介
====

核心特征
=========

1. 支持两种任务类型：第一种Curl模式，第二种PHP Cli模式，文件只能放在本地服务器。Cli方式又分为Yaf Cli模式和原生无任何框架Cli模式；
2. 任务执行方式分三种：第一种循环执行，设置间隔执行时间，可以精确到秒；第二种每天执行一次，设置每天固定时间执行；第三种只执行一次
3. 系统需要按照yaf（3.0.2），yaconf（1.0.1），swoole（1.9.10）扩展


目录结构介绍
=============

1. worker目录是计划任务系统目录，基于swoole开发；
2. web目录是任务管理系统后台，基于yaf开发，登录接入UAP；
3. yafCli是yaf cli模式， phpCli是php原生Cli模式；
4. vendor第三方类，通过composer来配置；src是本地需要用到的类；
5. config为配置目录，cron_application.ini为项目配置，cron_database.ini为数据库配置
6. log为日志目录
