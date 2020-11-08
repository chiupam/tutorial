# Single node

Users can add a self-built server through the `single node` button. A node represents a proxy server, and the proxy server can realize the transfer of traffic.

-Currently supported protocols are

  -HTTP
  
  -HTTPS
  
  -SS
  
  -SSR
  
  -V2ray
  
  -Trojan

# Add method

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon currently supports three UI methods to add a single node: manually enter the configuration, paste the URL, scan the QR code.

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Users can also enter the homepage, click on the bottom of `Configuration` -> `Single node` -> `+` to make related nodes Configuration.

# The first method: write through the UI

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click the `Configuration` column below, and click `Single node`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the area shown in the upper right corner (+)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Direct` on the right side of the agreement

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the required protocol and click to enter the configuration

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_UI_4.jpg)

# The second method: by writing in the `configuration file` or `text editor`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click the `Configuration` bar below, and click `Text Edit`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Conf_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Find `[Proxy]` and write in the next line

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Conf_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The format is as follows

```
[Proxy]
# Built-in DIRECT, REJECT strategy

# http(s)
# Node name = protocol, server address, server port, user name, password
1 = http, 1.2.3.4, 443, username, "password"
2 = https, 1.2.3.4, 443, username, "password"

# ss(r)
# Node name = protocol, server address, server port, encryption protocol, password
1 = Shadowsocks, 1.2.3.4, 443, aes-128-gcm, "password"
2 = Shadowsocks, 1.2.3.4, 443, aes-128-gcm, "password"
3 = ShadowsocksR, 1.2.3.4, 443, aes-256-cfb,"password",auth_aes128_md5,{},tls1.2_ticket_auth,{}
4 = ShadowsocksR, 1.2.3.4, 10076, aes-128-cfb,"password",auth_aes128_md5,{},tls1.2_ticket_auth,{}

# vmess
# Node name = protocol, server address, port, encryption method, UUID, transmission method: (tcp/ws), path: path in the websocket handshake header, host: path in the websocket handshake header, over-tls: whether tls, tls-name: tls name, skip-cert-verify: whether to skip certificate verification (default is no)
6 = vmess, 1.2.3.4, 10086, aes-128-gcm,"uuid",transport:ws,path:/,host:icloud.com,over-tls:true,tls-name:youtTlsServerName.com,skip- cert-verify:false

# trojan
#Node name = protocol, server address, port, password, tls-name: tls name, skip-cert-verify: whether to skip certificate verification (default is no)
7 = trojan, 1.2.3.4, 443,password,tls-name:youtTlsServerName.com,skip-cert-verify:false
```

# Say a few more words

- Due to different protocols, users need to write the configuration by themselves, this tutorial will not describe in detail

# Reference

- [Loon Incomplete Tutorial-Node Import](https://www.notion.so/1-9809ce5acf524d868affee8dd5fc0a6e#d8572e22c34e483589a445b174eec2bb)

- [LoonManual](https://github.com/Loon0x00/LoonManual/blob/master/README.md)