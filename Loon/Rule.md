# 订阅规则

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 本教程所说的订阅规则仅限订阅规则的策略选择为 DIRECT、PROXY（此名称不一定）、REJECT 时浏览，例如国内规则策略选择 DIRECT，去广告规则选择 REJECT 等

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 需要订阅特别 APP 的规则，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Rule_Netflix.md) 学习教程

## 一、复制订阅规则的 Raw 链接

首先找到用户需要订阅的规则，推荐使用 [Conners Hua](https://github.com/ConnersHua?tab=repositories) 的规则，点击 [这里](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset
) 前往 github 库

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 以订阅 China.list (国内规则) 规则为例，点击 China.list

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 Raw

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 长按地址栏，并复制/拷贝地址

## 二、进入 Loon 内订阅规则

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 订阅规则的策略选择分为三种，分别是 DIRECT、REJECT、PROXY，因为 China.list 是中国规则，所以这里策略选择为 DIRECT（直连），策略选择为 REJECT 、 PROXY 时是类似操作，这里不再阐述

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方配置栏，点击下图所示区域（订阅规则）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将上面复制/拷贝下来的地址粘贴到 URL 处，填写分流别名

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（DIRECT）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 DIRECT 即可

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（保存）

## 三、订阅规则的位次规定

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 订阅规则的位次是有规定的，顺序由上到下的顺序应该为

- 去广告类（策略选择 REJECT）

- 国内直连类（策略选择DIRECT）

- 国外特定 APP 代理（建议学习[此教程](https://github.com/chiupam/tutorial/blob/master/Loon/Rule_Netflix.md)）

- 国外代理类（策略选择 PROXY {此策略名字不一定，需要看配置具体而定}）
