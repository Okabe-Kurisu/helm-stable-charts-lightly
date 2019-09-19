## 为什么是helm-stable-charts-lightly？
因为现版本（2.2.7）应用商店在导入应用仓的时候存在内存泄漏问题。所以需要有一个内容较少的临时仓库。虽然这样既可以看到应用列表，又可以避免容器云宕机。但是这样的方法绝对不是长期方案，应该尽快想办法解决内存泄漏的问题才是。

## 怎么获取应用商店中某个应用的其他版本？
使用`rancher-tool`工具中的`tran`flag来进行移动，具体参见`rancher-tool`的README。

## 想要的应用连`helm-stable`中都不存在
按照`helm-stable`库中的README维护一下helm-stable