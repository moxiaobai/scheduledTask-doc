=================
任务系统web管理
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
