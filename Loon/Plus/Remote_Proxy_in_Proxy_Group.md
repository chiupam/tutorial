# 节点与策略组之间的嵌套

将代理节点添加到策略组下，实现代理功能

## 方法

打开 Loon 并点击下方 `配置` 栏，点击 `策略组`

点击需要添加代理节点的策略组，以下图所示中的 `手动选择` 策略组为例，点击 `手动选择`

点击并设置 `策略类型` ，分成 4种情况 

- 用户希望手动选择节点时，策略类型选择 `select`

- 用户希望自动选择最低延迟节点时，策略类型选择 `url-test` ，教程请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md) 跳转 

- 用户希望自动选择可用节点时，策略类型选择 `fallback` ，教程请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md) 跳转 

- 用户希望符合预设条件的节点自动对同一主机名的请求锁定同意节点时，先在策略类型选择 `load-balance` ，然后在负载均衡算法选择 `pcc` ，教程请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md) 跳转 
