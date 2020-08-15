# PCC

`PCC` 策略组可以通俗理解成 Loon 间隔一段时间自动测试`PCC` 策略组下节点延迟，并剔除用户设置最大延迟的节点，对用户发起的同一主机名的网络访问请求锁定同一节点

# 一、进入 `策略组` 添加策略组

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `策略组`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `select` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `load-balance` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `random`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `pcc`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Tes-URL` 一般不需要修改，`测试间隔` 的单位为 `秒` ， `最大超时` 的单位为 `毫秒` ，按用户个人使用习惯修改，推荐 `最大超时` 修改为 `1000`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `添加`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 从 `筛选订阅节点` 列表下选择筛选后的节点，严厉禁止从 `订阅节点` 列表下选择，否则会出现 Loon 警告，甚至是机场封号等严重后果

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `储存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 确保 `订阅筛选` 下 `筛选` 的 `()` 内有数字后点击 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/PCC_8.jpg)

# 多说几句

- 按本教程新增的 `PCC` 策略组没有实质性作用，需要将 `PCC` 策略组作为子策略组嵌套进代理母策略组中才会发挥实质性作用

- 添加代理节点时，严厉禁止从 `订阅节点` 列表下选择，否则会出现 Loon 警告，甚至是机场封号等严重后果

- `筛选订阅节点` 内也不允许有过多的节点，建议低于 `10` 个，否则也容易出现 Loon 警告，甚至是机场封号等严重后果

- 如果不会利用正则表达式筛选适合的节点，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Regex.md) 跳转学习正则表达式
