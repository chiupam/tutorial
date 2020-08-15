# 单个节点

用户可以通过 `单个节点` 按钮添加自行搭建的服务器

- 目前支持的协议有

  - HTTP
  
  - HTTPS
  
  - SS
  
  - SSR
  
  - V2ray
  
  - Trojan

# 第一种方法：通过UI写入

打开 Loon 并点击下方 `配置` 栏，点击 `单个节点`

点击右上角所示区域（+）

点击协议右侧 `Direct` 

选择需要的协议并点击进入配置

# 在配置中写入

```
[Proxy]
# 单个节点添加在下面
# SS 格式: 节点名称 = 协议，服务器地址，服务器端口，加密协议，密码
1 = Shadowsocks, 1.2.3.4, 443, aes-128-gcm, "password"
2 = Shadowsocks, 1.2.3.4, 443, aes-128-gcm, "password"

# SSR 格式：名称=协议类型,地址,端口,加密方式,密码,协议类型,{协议参数},混淆类型,{混淆参数}
3 = ShadowsocksR, 1.2.3.4, 443, aes-256-cfb,"password",auth_aes128_md5,{},tls1.2_ticket_auth,{}
4 = ShadowsocksR, 1.2.3.4, 10076, aes-128-cfb,"password",auth_aes128_md5,{},tls1.2_ticket_auth,{}

# vmess格式
# 节点名称 = 协议,服务器地址,端口,加密方式,UUID,传输方式:(tcp/ws),path:websocket握手header中的path,host:websocket握手header中的path,over-tls:是否tls,tls-name:远端w服务器域名,skip-cert-verify:是否跳过证书校验（默认否）
5 = vmess,1.2.3.4,10086,aes-128-gcm,"uuid",transport:ws,path:/,host:icloud.com,over-tls:true,tls-name:youtTlsServerName.com,skip-cert-verify:false

# http 格式 (不支持 username, password)
ProxyHTTP = http, 1.2.3.4, 8888
```

# 多说几句

- 由于协议的不同，需要用户自行写入配置，此教程不详细讲述
