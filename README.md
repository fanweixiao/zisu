## 环境需求
- PHP >= 5.5.9
- MySQL / MariaDB
- composer

安装后请确保可以通过命令 ``php -v`` ``composer -v`` 查看到两者的版本

## 安装
```
composer install  #自动安装需求环境
php artisan migrate  #执行数据库迁移 
```
#### 使用 PHP Cli_Server 驱动
```
cd public
php -S 0.0.0.0:80
```
#### 使用 Nginx / Apache 等驱动参照 Laravel 框架通用方法，将 /public 设置为工作根目录
完成上诉步骤后，访问 ```http://您的域名/install``` 完成最后安装

## 对接模块
- 本系统所有与服务器对接的模块放置于 ``/server/`` 下，目录名字即为后台所识别的模块名称
- 每一个完整的模块包含着 ``setings.php`` ``create.php`` ``delete.php`` ``start.php`` ``stop.php`` 五个文件。分别对应五个不同的操作。
- 模块制作规范请正在制作中，具体可以参照现有的 ep1 (与EasyPanel对接) 示例
##说明
-二开RyShop
