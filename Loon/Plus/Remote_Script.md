# 订阅脚本

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 订阅脚本通过读取 URL 内容，自动识别脚本语句和域名，批量在 Loon 内添加脚本

## 对 URL 格式及内容的要求

- 对 URL 格式的要求

  - 文件上传至github库的，订阅地址 URL 必须以 `http://raw` 开头
  
- 对 URL 内容的要求

  - 必须包含一条或以上脚本语句
  
  - 可以写有 `hostname =` 的语句
  
## URL 内容示范

```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true

hostname = example1.com,example2.com
```

## URL 实例文件示范

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 直接点击下方的地址，查看 URL 的内容的正确格式写法

https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/Remote_Script_Example.conf

## 获取正确的 URL 链接的方法

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击需要订阅脚本的文件

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 Raw

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 长按地址栏，点击 `拷贝` 即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_3.jpg)

## 订阅脚本

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `订阅脚本`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击如图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `URL` 栏粘贴用户获取的正确的 URL 链接

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `别名` 栏填入订阅脚本的命名，按用户个人喜爱命名

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击如图所示区域，更新 `订阅脚本` 即可完成操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_5.jpg)

# 多说几句

- 个人认为订阅脚本内只订阅一个脚本会显得有点折腾

  - 例如：[错误的订阅脚本方式](https://t.me/Loon0x00/350684)
  
# 鸣谢

- [NobyDa](https://github.com/NobyDa/Script/blob/master/JD-DailyBonus/JD_DailyBonus.js)

- [lxk0301](https://github.com/lxk0301/scripts/blob/master/jd_fruit.js)

- [chavyleung](https://github.com/chavyleung/scripts/tree/master/wmmeituan)
