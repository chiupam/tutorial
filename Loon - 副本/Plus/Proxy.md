# 单个节点

用户可以通过 `单个节点` 按钮添加自行搭建的服务器，一个节点代表一个代理服务器，代理服务器可以实现流量的中转。

- 目前支持的协议有

  - HTTP
  
  - HTTPS
  
  - SS
  
  - SSR
  
  - V2ray
  
  - Trojan

# 添加方法

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon 目前支持三种 UI 方式添加单个节点：手动输入配置、粘贴 URL、扫描二维码。 

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 用户也可以进入主页，点击下方 `配置`-> `单个节点` -> `+` 可进行相关节点配置。

# 第一种方法：通过UI写入

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `单个节点`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击右上角所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击协议右侧 `Direct` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择需要的协议并点击进入配置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_4.jpg)

# 第二种方法：通过在 `配置文件` 或 `文本编辑` 中写入

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `文本编辑`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Conf_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到 `[Proxy]` 并在其下一行写入

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Conf_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 格式如下所示

```
[Proxy]
# 内置 DIRECT、REJECT 策略

# http(s)
# 节点名称 = 协议，服务器地址，服务器端口，用户名，密码
1 = http, 1.2.3.4, 443, username, "password"
2 = https, 1.2.3.4, 443, username, "password"

# ss(r)
# 节点名称 = 协议，服务器地址，服务器端口，加密协议，密码
1 = Shadowsocks, 1.2.3.4, 443, aes-128-gcm, "password"
2 = Shadowsocks, 1.2.3.4, 443, aes-128-gcm, "password"
3 = ShadowsocksR, 1.2.3.4, 443, aes-256-cfb,"password",auth_aes128_md5,{},tls1.2_ticket_auth,{}
4 = ShadowsocksR, 1.2.3.4, 10076, aes-128-cfb,"password",auth_aes128_md5,{},tls1.2_ticket_auth,{}

# vmess
# 节点名称 = 协议，服务器地址，端口，加密方式，UUID，传输方式:(tcp/ws),path：websocket握手header中的path，host：websocket握手header中的path，over-tls:是否tls，tls-name：tls名字，skip-cert-verify：是否跳过证书校验（默认否）
6 = vmess, 1.2.3.4, 10086, aes-128-gcm,"uuid",transport:ws,path:/,host:icloud.com,over-tls:true,tls-name:youtTlsServerName.com,skip-cert-verify:false

# trojan
#节点名称 = 协议，服务器地址，端口，密码，tls-name：tls名字，skip-cert-verify：是否跳过证书校验（默认否）
7 = trojan, 1.2.3.4, 443,password,tls-name:youtTlsServerName.com,skip-cert-verify:false
```

# 多说几句

- 由于协议的不同，需要用户自行写入配置，此教程不详细讲述

# 参考

- [Loon 不完全教程 - 节点导入](https://www.notion.so/1-9809ce5acf524d868affee8dd5fc0a6e#d8572e22c34e483589a445b174eec2bb)

- [LoonManual](https://github.com/Loon0x00/LoonManual/blob/master/README.md)
