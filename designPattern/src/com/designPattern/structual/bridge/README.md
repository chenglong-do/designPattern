# 桥接模式

## 意图

将抽象部分与它的实现部分分离，使它们都可以独立变化。


## 解析


![](../../../../../img/bridge.png)

## 总结

将跟平台相关的实现抽象为一个统一的接口（IWindowImp），抽象部分（Window）是指跟平台无关的部分，这两部分都通过抽象建立依赖关系，这个依赖关系就像桥一样把两者关联起来，最终各部分可以独立变化。

需要注意的一点是抽象部分的接口不一定会和实现部分一致，实现部分提供的是基础功能，抽象部分对功能做组装扩展，从而实现用户的需求。

