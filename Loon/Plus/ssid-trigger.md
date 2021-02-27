# ssid-trigger

- 官方解析:

  - [TestFlight(262)](https://t.me/LoonNews/426)：[general]添加ssid-trigger参数，用于指定SSID下流量模式切换，参考样例如下： ssid-trigger="default":rule,"cellular":rule,"SYSLINY-Pro":direct,"TPLINK":proxy （default表示默认，cellular表示蜂窝，目前支持三种值：rule，direct，proxy）

- 小白理解：一种比[设置 ssid 内置策略组方案](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/ssid.md)和[设置自动脚本方案](https://t.me/cool_scripts/141)都更为快捷的ssid策略

## 注意

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 使用此方法设置 ssid 策略，务必需要用户知道已扶墙路由器的 SSID 是什么，如果不知道如何查看路由器 SSID 的用户，请自行百度或者参考[百度文库](https://wenku.baidu.com/view/9cfde0060166f5335a8102d276a20029bd64631f.html)

## 其他方法

- [内置 ssid 策略组的设置](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/ssid.md)

- [进阶操作 —— SSID 策略组嵌套教程](https://github.com/ArriettyQAQ/loon_tutorial)

- [脚本的方法](https://t.me/cool_scripts/141)

## 操作步骤

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 复制以下代码

> 代码意思为：默认情况下使用规则分流模式，蜂窝数据情况下使用规则分流模式，连接 SSID_1 无线网络情况下使用全局直连模式

```
ssid-trigger="default":rule,"cellular":rule,"SSID_1":direct
```

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon，点击下方 `配置` 栏

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid-trigger_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击文本配置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid-trigger_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到 `[general]` 配置栏

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid-trigger_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在其下面寻找合适的行粘贴第一步时复制的代码

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid-trigger_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 修改 `SSID_1` 成用户已扶墙路由器 SSID 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid-trigger_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击右上角的 `完成` 按钮即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid-trigger_6.jpg)

## 多说几句

- 使用此方法的设置在连接指定 Loon 使用全局直连模式的无线网络时，用户在 Loon 中预设的特定 APP 策略组会走路由器节点，请注意以下 APP

  - Netflix

  - Disney

  - ...

- 如果家中有多台路由器扶墙，请参考以下规律自行修改

```
ssid-trigger="default":rule,"cellular":rule,"SSID_1":direct,"SSID_2":rule,"SSID_3":proxy
```
