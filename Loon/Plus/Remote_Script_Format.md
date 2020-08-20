# 订阅脚本 URL 

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 此教程让用户统一学习关于订阅脚本中填写的 URL 的格式要求及其内容要求

## 一、对 URL 格式及其内容的要求

- 对 URL 格式的要求

  - 文件上传至github库的，订阅地址 URL 必须以 `http://raw` 开头
  
- 对 URL 内容的要求

  - 必须包含一条或以上脚本语句
  
  - 可以写有 `hostname =` 的语句
  
## 二、URL 内容示范

```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true

hostname = example1.com,example2.com
```

## 三、URL 实例文件示范

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 直接点击下方的地址，查看 URL 的内容的正确格式写法

https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/Remote_Script_Example.conf

## 四、获取正确的 URL 链接的方法

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击需要订阅脚本的文件

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 Raw

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 长按地址栏，点击 `拷贝` 即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_3.jpg)
