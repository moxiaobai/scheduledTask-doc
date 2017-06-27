===============
worker配置管理
===============

任务报警说明
=====================

1.任务报警间隔时间为20分钟一次
2.短信和邮件通知


应用配置(cron_application.ini)
===============================

::

 ;计划任务系统服务
 cronServer.host = 127.0.0.1
 cronServer.port = 9503

 ;yaf cli程序执行目录
 yafCli.directory = /mnt/www/scheduledTask_swoole/yafCli/

 ;php cli程序执行目录
 phpCli.directory = /mnt/www/scheduledTask_swoole/phpCli/


数据库配置(cron_database.ini)
==============================

