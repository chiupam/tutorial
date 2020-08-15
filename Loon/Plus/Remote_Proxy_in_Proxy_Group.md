# 节点与策略组之间的嵌套

将代理节点添加到策略组下，实现代理功能

## 一、

打开 Loon 并点击下方 `配置` 栏，点击 `策略组`

点击需要添加代理节点的策略组，以下图所示中的 `手动选择` 策略组为例，点击 `手动选择`

点击并设置 `策略类型` ，分成 4种情况 

- 用户希望手动选择节点时，策略类型选择 `select` ，请直接本教程下面的 `二`

- 用户希望自动选择最低延迟节点时，策略类型选择 `url-test` ，然后请浏览教程第二步以及第三步，点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md) 跳转 

- 用户希望自动选择可用节点时，策略类型选择 `fallback` ，然后请浏览教程第二步以及第三步，点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md) 跳转 

- 用户希望符合预设条件的节点自动对同一主机名的请求锁定同意节点时，策略类型选择 `load-balance` ，然后请浏览教程第二步以及第三步，点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md) 跳转 

## 二、仅供策略类型选择 `select` 时浏览

以策略类型选择 `select` 为例，点击 `添加`

从 `订阅节点` 或者 `筛选订阅节点` 的列表下选择需要的`订阅节点` 或者 `筛选订阅节点` ，点击名称

点击 `储存`

确保 `订阅筛选` 下 `筛选` 的 `()` 内有数字后点击 `保存`
