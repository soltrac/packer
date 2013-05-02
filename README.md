# Github Pages:
  
  [http://viennadd.github.io/packer/](http://viennadd.github.io/packer/)


## 简介
> 学习PE结构和加壳流程的作品

> 没有处理资源表

> 不支持tls callback

> dll无力

> 只压缩，无加密和反调试

***

## 流程大概是：

1. 载入PE和stub.dll

1. 新增区段放stub的代码段（包含stub导入表和stub数据）

1. 使用stub的重定位表重定位一下stub

1. 产物使用stub的导入表

1. Tls单纯搞块00，原本有的callback会丢失

1. 各区段原地压缩

***


## stub流程:

1. 解压

1. 填充iat

1. 跳到OEP

***

## 致谢
> 感谢看雪各种时期大牛们的资料分享

> 感谢零下安全的群友们指导与帮助


