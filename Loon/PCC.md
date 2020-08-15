# PCC

`PCC` 策略组可以通俗理解成 Loon 间隔一段时间自动测试`PCC` 策略组下节点延迟，并剔除用户设置最大延迟的节点，对用户发起的同一主机名的网络访问请求锁定同一节点

# 一、进入 `策略组` 添加策略组

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `策略组`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `select` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL-Test_1.jpg)

点击 `load-balance` 

点击 `random`

点击 `pcc`

`Tes-URL` 一般不需要修改，`测试间隔` 的单位为 `秒` ， `最大超时` 的单位为 `毫秒` ，按用户个人使用习惯修改，推荐 `最大超时` 修改为 `1000`

点击 `添加`

订阅

点击 `储存`

确保 `订阅筛选` 下 `筛选` 的 `()` 内有数字后点击 `保存`
