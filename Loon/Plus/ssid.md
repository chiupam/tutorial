# 内置 ssid 策略组

有一些用户使用路由器扶墙，希望 Loon 的代理分流可以自动切换成直连状态，不需要用户手动进入 Loon 中开启全局直连模式，这时候可以使用 Loon 内置的 ssid 策略组

## 注意

Loon 内置的 ssid 策略组的嵌套有一定的理解难度，此教程需要用户明白规则的作用、代理策略组的概念，下方提供教程链接

- [何为规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule_Summary.md)

- [代理策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy.md)

打开Loon，点击下方配置栏
点击策略组
点击右上角+
在别名栏输入策略组名称，推荐使用SSID即可
点击策略类型
选择ssid
点击默认
推荐选择代理策略组
点击蜂窝数据
推荐选择代理策略组
点击添加
输入用户已扶墙的路由器名称
然后点击确定
选择DIRECT
点击右上角保存
