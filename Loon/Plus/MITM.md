# MITM （Man in the Middle Attack）

Loon 利用中间人攻击的方式解密 https 的请求。根据配置的 hostname（域名） 和信任的 CA 证书解密相应的 https 请求和响应，解密后可以配合 Rule 和 URL Rewrite 进行分流。

# 多说几句

- 了解更多MITM的知识

  - [维基百科 —— MTIM](https://zh.wikipedia.org/wiki/%E4%B8%AD%E9%97%B4%E4%BA%BA%E6%94%BB%E5%87%BB)

  - [百度百科 —— MITM](https://baike.baidu.com/item/%E4%B8%AD%E9%97%B4%E4%BA%BA%E6%94%BB%E5%87%BB/1739730?fr=aladdin)

- 传送门

  - [CA证书](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Certificate.md)

  - [hostname](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/hostname.md)