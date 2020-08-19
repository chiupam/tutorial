# 节点与策略组之间的嵌套

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将代理节点添加到策略组下，实现代理功能

## 一、初步设置

- 用户未曾添加一个策略组作为 `代理策略组` 嵌套节点，，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md) 跳转 `新建子策略组` 教程学习如何添加一个策略组

- 用户已经成功添加一个策略组作为 `代理策略组` 嵌套节点，请继续浏览以下教程

---

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `策略组`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Group.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击需要添加代理节点的策略组，以下图所示中的 `手动选择` 策略组为例，点击 `手动选择`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Proxy_in_Proxy_Group_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击并设置 `策略类型` ，分成 4种情况 

- 用户希望手动选择节点时，策略类型选择 `select` ，请直接本教程下面的 `二`

- 用户希望自动选择最低延迟节点时，策略类型选择 `url-test` ，然后请浏览教程第二步以及第三步，点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md) 跳转 

- 用户希望自动选择可用节点时，策略类型选择 `fallback` ，然后请浏览教程第二步以及第三步，点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md) 跳转 

- 用户希望符合预设条件的节点自动对同一主机名的请求锁定同意节点时，策略类型选择 `load-balance` ，然后请浏览教程第二步以及第三步，点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/PCC.md) 跳转 

## 二、仅供策略类型选择 `select` 时浏览

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 以策略类型选择 `select` 为例，点击 `添加`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Select_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 从 `订阅节点` 或者 `筛选订阅节点` 的列表下选择需要的`订阅节点` 或者 `筛选订阅节点` ，点击名称

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Select_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `储存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Select_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 确保 `订阅筛选` 下 `筛选` 的 `()` 内有数字后点击 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Select_4.jpg)

# 多说几句

- 仅当策略类型选择 `select` 时才可以从 `订阅节点` 列表下选择，其余策略类型都严厉禁止从 `订阅节点` 列表中选择


