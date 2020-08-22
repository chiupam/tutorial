# 网络共享

Q：我有两台设备，我在其中一台设备下载了 Loon ，能不能让另一台设备在不下载 loon 的情况下实现科学上网？

A：可以通过 `网络共享` 功能实现。

## 网络共享的作用

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon 向 Wi-Fi 下的其他设备提供一个 HTTP/SOCKET5 代理服务器，让处于同一个 Wi-Fi 下的其他设备，通过用户在其他设备中手动设置 HTTP 代理端口和服务器实现科学上网

## 开启此功能的必要条件

- A设备（已经下载 Loon 的设备）

  - 必须开启 无线局域网 / Wi-Fi 功能并连接一个 Wi-Fi
  
  - Loon 中必须开启 `网络共享` 功能
  
- B设备（没有下载 Loon 的设备）

  - 必须开启 无线局域网 / Wi-Fi 功能并连接与 A设备 同一个 Wi-Fi
  
  - 手动设置 HTTP 代理配置
  
## 一、添加 `网络共享` 快捷方式至 Loon 的`仪表` 栏界面内

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 界面并点击 `快捷方式` 右侧指定区域

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 长按 `不可见` 列表下的 `网络共享` 右侧指定区域，拖动直 `可见` 列表下

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 确定 `可见` 列表出现 `网络共享` ，然后点击 `返回`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_2.jpg)

## 二、在已经下载 Loon 的 A设备 的操作步骤

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 Loon 界面的 `网络共享` 的卡片开关，开启 `网络共享` 功能

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 务必将 `网络共享` 卡片下的 **灰色ip地址（即服务器）** 记录下来，且此处没有出现 `⛔️` 表情包

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 Loon 界面内点击 `网络共享` 卡片

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 务必将 `HTTP代理端口` 记录下来，然后请继续操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_6.jpg)

## 三、在没有下载 Loon 的 B设备 的操作步骤

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 B设备内 `设置` ，点击 无线局域网 / Wi-Fi ，开启 无线局域网 / Wi-Fi 功能

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 连接与 A设备 同一个 无线局域网 / Wi-Fi

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击如图所示区域

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到 `HTTP代理` 列表并点击 `配置代理`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择 `手动`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `服务器` 栏填写 A设备的 Loon 中 `网络共享` 卡片下的 `灰色ip地址`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `端口` 栏填写 A设备的 Loon 中 `网络共享` 卡片内的 `HTTP代理端口`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `存储` 即可实现 B设备 的科学上网

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_8.jpg)

# 多说几句

- 需要第一步操作的原因是 Loon 的 `配置` 栏内没有 `网络共享` UI ，目前只能通过以下两种方式开启 `网络共享` 功能

  - `网络共享` 卡片
  
  - `文本配置` 内写入相关代码（此方法已过时）

- 对于 A设备 开启 `网络共享` 功能后，在 `网络共享` 卡片下方出现 `⛔️` 表情包，请开启  无线局域网 / Wi-Fi 功能并连接一个 Wi-Fi

- 对于 B设备 不能通过此功能在某些 APP 上实现科学上网的，可能是这类 APP 上使用的是 ` SOCKET5代理` ，请自行在这类 APP 内设置功能内手动配置 SOCKET5 代理的服务器和端口
