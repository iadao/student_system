# school
基于thinkphp6.0+mysql+bootstrap4的疫情防控系统毕业设计

运行环境
thinkphp6.0
mysql5.7
bootstrap4
本地测试集成环境软件：phpstudy
安装
可参考thinkphp项目搭建
添加网站根目录/public
添加伪静态

<IfModule mod_rewrite.c>
Options +FollowSymlinks -Multiviews
RewriteEngine on
RewriteBase /
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^(.*)$ index.php?s=/$1 [QSA,PT,L]
</IfModule>


导入数据库
修改数据库配置/app/config/database.php
若项目无法启动删除runtime再试
