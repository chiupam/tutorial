# 订阅分流并选择策略

Q：我想在我使用 Netflix 时代理选择奈菲节点，我该如何操作？

A：通过订阅规则，选择策略，达到想要的效果。

## 一、新建策略（是的，就是新建策略）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Proxy_Group.md) 完成新建策略组的操作

## 二、订阅规则/分流（分流是 Quantumult X 的叫法）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先复制/拷贝右侧这串地址：https://raw.githubusercontent.com/ConnersHua/Profiles/master/Surge/Ruleset/Media/Netflix.list

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（订阅规则）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（+）并确保订阅的 Netflix 规则处于的位置最低不得低于国际媒体规则之下

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将上面复制/拷贝下来的地址粘贴到 URL 处，填写分流别名

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（DIRECT）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择刚刚创建的 Netflix 策略组

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 正确配置如下图所示，然后点击下图所示区域（保存）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_6.jpg)

## 三、查看 Netfix 策略组情况

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（策略组）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（Netflix）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如果没有蓝色节点出现则手动选择一个

## 多说几句

- 订阅规则是有先后顺序的，访问请求匹配的订阅规则依次从上到下进行匹配

- ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如下图所示，如果 Netflix 订阅规则位于国际媒体订阅规则之上，打开 Netflix 时走 Netflix 策略组下节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_8.jpg)

- ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如下图所示，如果国际媒体订阅规则位于 Netflix 订阅规则之上，打开 Netflix 时走 Proxy 策略组下节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_9.jpg)

- ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如果需要添加更多分流，却不知道从哪里找，在这里推荐 ConnersHua 的订阅规则，请点击 [这里](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset) 跳转

# 鸣谢

- [ConnersHua](https://github.com/ConnersHua) 提供的分流
