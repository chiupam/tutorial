# `订阅规则` 功能存在的必要性和优点

`订阅规则` 可以让用户免需在本地规则中手动添加一个又一个的规则，社区有大佬整理了各种规则供用户订阅，省去用户自行本地添加规则的麻烦

## 一、复制订阅规则的 Raw 链接

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 首先找到用户需要订阅的规则，推荐使用 [Conners Hua](https://github.com/ConnersHua?tab=repositories) 的规则，点击 [这里](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset) 前往 github 库

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 以订阅 `China.list` (国内规则) 规则为例，点击 `China.list`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_Raw_China_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `Raw`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_Raw_China_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `拷贝`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_Raw_China_3.jpg)

## 二、确定 `订阅规则` 所选策略

订阅规则的策略选择分为三种，分别是

- `DIRECT`

- `REJECT`

- `代理策略组`

- `母策略组`

因为 `China.list` 是中国规则，所以这里策略选择为 `DIRECT`（直连），策略选择为 `REJECT` 、 `代理策略组` 、 `母策略组` 时是类似操作，这里不再阐述


## 三、进入 Loon 内订阅规则

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方 `配置` 栏，点击 `订阅规则`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将上面复制/拷贝下来的地址粘贴到 `URL` 处，填写分流别名

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `DIRECT`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择 `DIRECT` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `保存` 即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_remote_China_6.jpg)

## 四、订阅规则的位次规定

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 订阅规则的位次是有规定的，顺序由上到下的顺序应该为

- 去广告类（策略选择 `REJECT`）

- 国内直连类（策略选择 `DIRECT`）

- 国外特定 APP 代理（策略选择  `代理策略组` 或者 `母策略组` {此策略名称每个用户不一定相同，需要看用户具体设置的名称而定}）

- 国外代理类（策略选择  `代理策略组` 或者 `母策略组` {此策略名称每个用户不一定相同，需要看用户具体设置的名称而定}）

# 多说几句

- 去广告规则推荐订阅 NobyDa 野比的去广告规则，github 库请点击 [这里](https://github.com/NobyDa/Script/tree/master/Surge) 跳转

- 流媒体规则推荐订阅 Conners Hua 的规则，github 库请点击 [这里](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset) 跳转

- 为什么说  `代理策略组` 或者 `母策略组`  名称每个用户不一定相同，需要看用户具体设置的名称而定，想了解原因请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Global_Policy.md) 跳转并阅读 `三、代理策略`

# 鸣谢

- [Conners Hua](https://github.com/ConnersHua?tab=repositories)

- [NobyDa](https://github.com/NobyDa)
