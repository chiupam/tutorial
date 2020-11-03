# URL-Test

`URL-Test` 策略组可以通俗理解成 Loon 间隔一段时间自动测试 `URL-Test` 策略组下节点延迟，并自动为用户选择最低延迟的节点

- [TestFilght 2.14(215)](https://t.me/LoonNews/287) 更新：添加 tolerance 参数，用于对比切换节点内时的容差，计算方式如下：前一次测速最优节点耗时-减去当前测速最优节点耗时大于 tolerance 时才会进行节点切换，默认100

  - 在 Loon 的更新说明中，对于此部分的描述为“小于”是错误的，正确应该为“大于”

## 一、进入 `策略组` 添加策略组

请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md) 跳转到 `手动添加一个策略组` 教程，完成操作后返回设置 `URL-Test` 教程

## 二、设置 `策略类型`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `select` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `url-test`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 按用户个人喜爱填入策略组别名，测试间隔单位为 `秒` ，按用户个人使用习惯修改，一般也不需要修改

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `容差` 栏根据用户个人喜爱和机场一般延迟自行设置，计算方法上边已有介绍，自行理解自行设置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Test-URL` 一般不需要修改

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_4.jpg)

## 三、添加代理节点

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 策略组是不能进行延迟测速的，因而只能添加代理节点

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 承接第一步的后面，点击 `添加`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 从 `筛选订阅节点` 列表下选择筛选后的节点，严厉禁止从 `订阅节点` 列表下选择，否则会出现 Loon 警告，甚至是机场封号等严重后果

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `储存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 确保 `订阅筛选` 下 `筛选` 的 `()` 内有数字后点击 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_8.jpg)

# 多说几句

- 按本教程新增的 `URL-Test` 策略组没有实质性作用，需要将 `URL-Test` 策略组作为子策略组嵌套进代理母策略组中才会发挥实质性作用

- 一定要注意的是 `URL-Test` 策略组下不可以嵌套其他子策略组，因为策略组不是节点，策略组没有延迟测试一说

- 添加代理节点时，严厉禁止从 `订阅节点` 列表下选择，否则会出现 Loon 警告，甚至是机场封号等严重后果

- `筛选订阅节点` 内也不允许有过多的节点，建议低于 `10` 个，否则也容易出现 Loon 警告，甚至是机场封号等严重后果

- 如果不会利用正则表达式筛选适合的节点，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md) 跳转学习正则表达式
