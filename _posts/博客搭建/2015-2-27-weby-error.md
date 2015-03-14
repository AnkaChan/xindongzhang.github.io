---
layout: post
category: 博客搭建
title: WebPy 0.3 常见错误
---

### AttributeError: 'module' object has no attribute 'inet_pton'

* 解决方法，修改Python安装目录下Lib\site-packages\web\net.py文件的第32到第35行为如下内容：

~~~~~~

    try:
        socket.inet_pton(socket.AF_INET6, address)
    except:
        return False
        
~~~~~~

### 链接数据库出错（XMAPP）（具体细节略）

* 注意在mysql创建对应的数据库，并且创建数据库中对应的table


### 链接数据库出错 （MySQL+webpy）

* 注意检查自己是否安装MySQL
* 检查MySQL中的item，也就是数据库的库名
* db = web.database(dbn='mysql', db='your-MySQL-item-name', user='root', pw='your-MySQL-password')，就能链接上数据库

### 默认端口0.0.0.0:8080无法访问
* 原因：端口被占用
* 解决：制定其他端口，如在cmd中运行python yourPythonfiles.py

### MySQL创建TABLE失败
* 原因：不合法的syntax
* 解决：查看版本对应争取的syntax，将MySQL的bin目录下的mysql.exe的路径配到环境目录下，然后命令行进行创建。 $ mysql -uroot -pyourpassword yourMySQL < yourtables.sql

