# 策略组之间的嵌套

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 无论 `Surge` `Quantumult X` `Loon` 这三个代理软件，在策略组的问题上，它们都是 `俄罗斯套娃` 来实现层层包装的

## 正确嵌套示范

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 本教程仅让用户在策略组与策略组之间嵌套，如若想让 Loon 使用子策略组内节点，需要正确嵌套母策略组与子策略组，正确的两种示范如下：

- 订阅规则 >>> 母策略组 >>> 子策略组 >>> 订阅节点/筛选订阅节点

- 订阅规则 >>> 母策略组 >>> 子策略组 >>> 次子策略组 >>> 订阅节点/筛选订阅节点

## 步骤

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如若想让 `手动选择` 策略组嵌套在 `Proxy` 策略组下，即 `Proxy` >>> `手动选择` ，如果用户没有创建 `Proxy` 策略组，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md) 跳转到 `新建策略组` 教程

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `策略组`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Group.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `Proxy` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Matryoshka_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 策略组之间的嵌套中 `策略类型` 只允许选择 `select` ，确认 `策略类型` 右侧为 `select` ，否则请修改此选项

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Matryoshka_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `添加`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Matryoshka_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 从 `策略组` 列表下点击 `手动选择` 策略组

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Matryoshka_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `存储`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Matryoshka_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在下方查看 `手动选择` 策略组是否有显示，然后点击 `保存` 即可完成嵌套操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Matryoshka_6.jpg)

# 多说几句

- 为了充分理解 `正确嵌套示范` 步骤，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/TOP_Policy.md) 学习 `正确分辨母策略组和子策略组`

- 策略组之间的嵌套中 `策略类型` 只允许选择 `select`
