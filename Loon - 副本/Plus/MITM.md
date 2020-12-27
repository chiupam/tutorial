# MITM （Man in the Middle Attack）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon 利用中间人攻击的方式解密 https 的请求。根据配置的 hostname（域名） 和信任的 CA 证书解密相应的 https 请求和响应，解密后可以配合 Rule 和 URL Rewrite 进行分流。

## MITM 的一般使用

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 用户在一般的使用中，如果不开启 MITM 功能，可能会使用户无法正确执行某些脚本，例如获取京东Cookie的脚本。

# 多说几句

- 了解更多关于 MITM 的知识

  - [维基百科 —— MTIM](https://zh.wikipedia.org/wiki/%E4%B8%AD%E9%97%B4%E4%BA%BA%E6%94%BB%E5%87%BB)

  - [百度百科 —— MITM](https://baike.baidu.com/item/%E4%B8%AD%E9%97%B4%E4%BA%BA%E6%94%BB%E5%87%BB/1739730?fr=aladdin)

- 传送门

  - [CA证书](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/CA.md)

  - [hostname](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/hostname.md)