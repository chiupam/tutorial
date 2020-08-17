# 什么是规则

![#f03c15](https://placehold.it/15/f03c15/000000?text=+)规则，决定了当一个请求进来时，如何通过匹配类型进行匹配，以及如何选用对应的策略

## 为什么代理软件要设置规则

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 因为使用代理软件时，用户访问防火墙内网站是不需要经过代理节点的，而当用户试图访问防火墙外的网站时是需要经过代理节点才能访问

   - 如：中国大陆用户直连访问 `www.baidu.com` 会成功，直连 `www.google.com` 则会失败，但是设置规则后，利用代理节点访问 `www.google.com` 就成功

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `自动分流` 模式下，为了让 Loon 能按需使用代理节点，必须为 Loon 设置规则

## 规则组成

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 规则分为三个部分，分别是：匹配类型 ，匹配内容，策略名称

   - 如： `DOMAIN-SUFFIX,twimg.com,PROXY`

## 匹配类型

匹配名称|匹配类型|说明
-|-|-
基于域名后缀|DOMAIN-SUFFIX|无
基于域名完整匹配|DOMAIN|无
基于域名关键字|DOMAIN-KEYWORD|无
基于用户代理串|USER-AGENT|根据 Http 的 user-agent 值来进行匹配，支持带有 \* , ? 的通配符匹配
基于URL正则|URL-REGEX|无
基于请求IP范围|IP-CIDR|通常用作局域网匹配
基于IP定为国家编码|GEOIP|CN中国
兜底匹配|FINAL|如果没有匹配的规则，默认使用的匹配

## 实例示范理解规则的作用

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如下图中的用户发起对 `www.google.com` 的一个访问请求中

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Ruld_Example.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `策略` 栏中， `Proxy` 代表策略， `[隧道]香港01#GZCM` 代表代理节点

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `规则` 栏中，`DOMAIN-KEYWORD` 代表匹配类型， `google` 代表匹配内容， `Proxy` 代表策略名称

即代表，用户发起对 `www.google.com` 的一个访问请求，被匹配类型为 `DOMAIN-KEYWORD` 域名关键字匹配，匹配内容为 `google` ，使用名为 `Proxy` 策略，该策略内最下层代理节点是 `[隧道]香港01#GZCM`

# 多说几句

- 兜底匹配，FINAL规则，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Final.md) 跳转到 `Final规则` 教程

# 参考

- [Loon 不完全教程 —— 规则-Rule](https://www.notion.so/2-967c1a07462c43ab88906162bec475a4)
