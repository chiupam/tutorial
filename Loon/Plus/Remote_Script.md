# 订阅脚本

订阅脚本通过读取 URL 内容，自动识别脚本语句和 hostname ，批量在 Loon 内添加脚本

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

直接点击下方的地址，查看正确的格式

https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/Remote_Script_Example.conf

## 获取正确的 URL 链接的方法

点击需要订阅脚本的文件

点击 Raw

长按地址栏，点击 `拷贝` 即可

## 订阅脚本

打开 Loon 并点击下方 `配置` 栏，点击 `订阅脚本`

点击如图所示区域（+）

在 `URL` 栏粘贴用户获取的正确的 URL 链接

在 `别名` 栏填入订阅脚本的命名，按用户个人喜爱命名

点击 `保存`

点击如图所示区域，更新 `订阅脚本` 即可完成操作

# 多说几句

- 个人认为订阅脚本内只订阅一个脚本会显得有点折腾

  - 例如：[错误的订阅脚本方式](https://t.me/Loon0x00/350684)
  
# 鸣谢

- [NobyDa](https://github.com/NobyDa/Script/blob/master/JD-DailyBonus/JD_DailyBonus.js)

- [lxk0301](https://github.com/lxk0301/scripts/blob/master/jd_fruit.js)

- [chavyleung](https://github.com/chavyleung/scripts/tree/master/wmmeituan)
