---
layout: post
category: 博客搭建
title: WebPy 0.3 常见错误
---

### AttributeError: 'module' object has no attribute 'inet_pton'

* 解决方法，修改Python安装目录下Lib\site-packages\web\net.py文件的第32到第35行为如下内容：

```

    try:
        socket.inet_pton(socket.AF_INET6, address)
    except:
        return False

```

### 链接数据库出错（具体细节略）

* 注意在mysql创建对应的数据库，并且创建数据库中对应的table


