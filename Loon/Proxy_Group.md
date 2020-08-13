# 策略组

此教程让用户明白如何添加一个策略组，并如何让自己创建的策略组发挥功能

## 一、新建策略组

（这一步教程只是让用户成功添加一个策略组，但是该策略组没有任何实质的功能，需要搭配下面的教程才会让策略组发挥效果）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（策略组）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 填写策略组名称（别名），策略类型下面再讲

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 添加可用策略，选择另外一个策略组或者节点，本教程选择最下面的筛选订阅节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（保存）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 至此，成功新建一个策略组

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如果是从分流教程跳转，需要回到分流教程的，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Rule_Netflix.md)

## 二、套娃（是的，就是套娃）

（请理解一下这句话：每个策略追溯至最上层策略，都会有一个分流在发生效果，因为刚刚新建的策略组没有被其他已经生效策略或订阅规则选为子策略，所以刚刚新建的策略只是一个空壳，没有任何实质的功能）

（下面只教让新建的策略组成为其他已经生效策略组的子策略组{有点拗口，多读几次}的方法）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（策略组）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（编辑）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（手动选择）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（添加），以添加另外一个策略组或者节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_8.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（Netflix），然后点击存储

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（保存）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_10.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（策略组）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_11.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域（手动选择），然后点击 Netflix

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_12.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 自此，手动选择策略组会使用 Netflix 策略组选择的节点，新建的 Netflix 策略组成功完成套娃工作

## 进阶教程：简单解释策略类型

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select：全手动选择，用户选择哪个节点，Loon 就使用哪个节点

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) URL-Test：通过指定的 URL 对节点进行延迟测试（注意是测试延迟并非速度）并自动选择最低延迟的节点，默认频率为600秒（可自行修改）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Fallback：通过指定的 URL 对节点进行可用性测试，并按照可用节点的排序自动选择第一个可用节点，默认频率为600秒（可自行修改）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Load-Balance：PCC ：通过指定的 URL 对节点进行延迟测试，排除超过设置延迟的节点，对发起相同主机名的访问请求锁定同一节点

# 多说几句

- 因为此教程搭配了订阅规则的教程一起使用，所以在第一步和第二步的时候选择的策略组名皆命名为 Netflix ，实际可以根据用户的需求自行定义策略组名称
