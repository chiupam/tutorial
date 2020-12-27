# 内置 ssid 策略组

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 有一些用户使用路由器扶墙，希望 Loon 的代理分流可以自动切换成直连状态，不需要用户手动进入 Loon 中开启全局直连模式，这时候可以使用 Loon 内置的 ssid 策略组

## 注意

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon 内置的 ssid 策略组的嵌套有一定的理解难度，此教程需要用户明白规则的作用、代理策略组的概念，下方提供教程链接

- [何为规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule_Summary.md)

- [代理策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy.md)

## 操作步骤

操作步骤分为两步，第一步是新建 ssid 策略组，第二部是更改订阅规则的策略组选择

### 新建 ssid 策略组

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon，点击下方 `配置` 栏

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `策略组`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击右上角 +

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在别名栏输入策略组名称，推荐输入 SSID 即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `策略类型`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择 `ssid`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `默认`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 推荐选择代理策略组，原因请看本教程下面的解析

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_8.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `蜂窝数据`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 推荐选择代理策略组

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_10.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `添加`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_11.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 输入用户已扶墙的路由器名称

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_12.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 然后点击 `确定`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_13.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择 `DIRECT`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_14.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击右上角 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_15.jpg)

### 更改订阅规则的策略组选择

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开Loon，点击下方 `配置` 栏

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `订阅规则`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择需要代理的分流，例如图示中的 `Global` 分流，原因请看本教程下面的解析

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 左滑该规则

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `编辑`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `策略`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择刚刚创建的 ssid 策略组，即名为 SSID 的策略组

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击右上角 `保存`即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_8.jpg)

## 多说几句

- 解析一下：

  - `默认` 中选择代理策略组是因为当用户连接到一个没有设置到的而且没有路由器扶墙的 WiFi 时，Loon 还是需要用分流模式，否则用户无法代理
  
  - `Global` 订阅规则是需要代理才可以访问成功的规则，所以每一个需要使用代理节点的订阅规则都需要进行第二步操作，否则很可能起不到用户想要的效果
  
  - 在懒人配置文本中，代理策略组的名字一般会命名为 Proxy
  
  - 如果用户使用自定义的配置文本，请根据自身情况选择代理策略组

- 如果用户想设置某些 APP ，例如 YouTube ，在使用路由器扶墙的时候走直连，方法是类似的，只是在第二步的操作中选择的规则是 YouTube 的订阅规则

- 如果订阅规则下的策略组为 DIRECT(直连) 或者 REJECT(拒绝)时，不要进行第二步，理由是：举个例子，大陆内用户在使用微信时，总不会使用代理节点吧？
