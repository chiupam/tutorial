# Fallback

`Fallback` 策略组可以通俗理解成 Loon 间隔一段时间自动测试 `Fallback` 策略组下节点是否可用，并依照节点排列自动选择第一个可用节点

## 一、进入 `策略组` 添加策略组

请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md) 跳转到 `手动添加一个策略组` 教程，完成操作后返回设置 `Fallback` 教程

## 二、设置 `策略类型`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `select` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `Fallback`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 按用户个人喜爱填入策略组别名， `测试间隔` 的单位为 `秒` ， `最大超时` 的单位为 `毫秒` ，按用户个人使用习惯修改，推荐 `最大超时` 修改为 `1000`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Test-URL` 一般不需要修改

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_3.jpg)

## 三、添加代理节点

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 策略组是不能进行延迟测速的，因而只能添加代理节点

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 承接第一步的后面，点击 `添加`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 从 `筛选订阅节点` 列表下选择筛选后的节点，严厉禁止从 `订阅节点` 列表下选择，否则会出现 Loon 警告，甚至是机场封号等严重后果

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `储存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 确保 `订阅筛选` 下 `筛选` 的 `()` 内有数字后点击 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_7.jpg)

# 多说几句

- 按本教程新增的 `Fallback` 策略组没有实质性作用，需要将 `Fallback` 策略组作为子策略组嵌套进代理母策略组中才会发挥实质性作用

- 一定要注意的是 `Fallback` 策略组下不可以嵌套其他子策略组，因为策略组不是节点，策略组没有延迟测试一说

- 添加代理节点时，严厉禁止从 `订阅节点` 列表下选择，否则会出现 Loon 警告，甚至是机场封号等严重后果

- `筛选订阅节点` 内也不允许有过多的节点，建议低于 `5` 个，否则也容易出现 Loon 警告，甚至是机场封号等严重后果

- 如果不会利用正则表达式筛选适合的节点，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md) 跳转学习正则表达式
