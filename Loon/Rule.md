# 订阅规则

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 本教程所说的订阅规则仅限订阅规则的策略选择为 `DIRECT`、`PROXY`（此名称不一定）、`REJECT` 时浏览，例如国内规则策略选择 `DIRECT`，去广告规则选择 `REJECT` 等

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 需要订阅特别 APP 的规则，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Rule_Netflix.md) 学习教程

## 一、复制订阅规则的 Raw 链接

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 首先找到用户需要订阅的规则，推荐使用 [Conners Hua](https://github.com/ConnersHua?tab=repositories) 的规则，点击 [这里](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset) 前往 github 库

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 以订阅 `China.list` (国内规则) 规则为例，点击 `China.list`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_Raw_China_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `Raw`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_Raw_China_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 长按地址栏，并复制/拷贝地址

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_Raw_China_3.jpg)

## 二、进入 Loon 内订阅规则

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 订阅规则的策略选择分为三种，分别是 `DIRECT`、`REJECT`、 `代理策略组` (此策略的名称不一定，需要看用户设置的具体名称而定)，因为 China.list 是中国规则，所以这里策略选择为 `DIRECT`（直连），策略选择为 `REJECT` 、 `代理策略组` (此策略的名称不一定，需要看用户设置的具体名称而定) 时是类似操作，这里不再阐述

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方 `配置` 栏，点击 `订阅规则`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将上面复制/拷贝下来的地址粘贴到 `URL` 处，填写分流别名

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `DIRECT`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `DIRECT` 即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_6.jpg)

## 三、订阅规则的位次规定

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 订阅规则的位次是有规定的，顺序由上到下的顺序应该为

- 去广告类（策略选择 `REJECT`）

- 国内直连类（策略选择 `DIRECT`）

- 国外特定 APP 代理（策略选择 `代理策略组` {此策略名字不一定，需要看用户设置的具体名称而定）

- 国外代理类（策略选择 `代理策略组` {此策略名字不一定，需要看用户设置的具体名称而定}）

# 多说几句

-  `代理策略组` 的名字不是每位用户都相同，需要看用户设置的具体名称而定，更多关于 `代理策略组` 的教程，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy.md) 跳转到 `代理策略组` 教程

- 去广告规则推荐订阅 NobyDa 野比的去广告规则，github 库请点击 [这里](https://github.com/NobyDa/Script/tree/master/Surge) 跳转

- 流媒体规则推荐订阅 Conners Hua 的规则，github 库请点击 [这里](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset) 跳转

- 还有更多订阅规则，请查看下方鸣谢处

# 鸣谢

- [Conners Hua](https://github.com/ConnersHua?tab=repositories)

- [NobyDa](https://github.com/NobyDa)

- [lhie1](https://github.com/lhie1/Rules/tree/master/Surge/Surge%203)

- [DivineEngine](https://github.com/DivineEngine/Profiles/tree/master/Surge/Ruleset)

- [eHpo1](https://github.com/eHpo1/Rules/tree/master/Surge4/Ruleset)
