=================
web管理
=================


nginx配置
====================

nginx.config

::

   server {
       listen 8989;
       root   /data/wwwroot/scheduledTask_swoole/web;
       index  index.html index.php;
    
       if (!-e $request_filename) {
          rewrite ^/(.*) /index.php?$1 last;
       }
    
      include enable-php.conf;
   }


网站配置
=======================

web/config/aplicaiton.ini修改app.host

::

  app.host = http://192.168.1.80:8989
