# 对 `http-request` 、 `http-response` 以及 `cron` 语句格式的基本认识

- `http-request` 语句，示例：
```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
```
  - `http-request` <===> 固定格式，表明语句类型
  
  - `^https?:\/\/(www.)?(example)\.com` <===> 正则表达式匹配到地址时执行脚本
  
  - `script-path=` <===> 固定格式，后接脚本路径
  
  - `localscript.js` <===> 脚本路径
  
  - `tag =` <===> 固定格式，意思为：标签，即用户将该语句自定义名称
  
  - `requestScript` <===> 脚本名称，按用户个人喜爱命名即可
  
  - `enable=` <===> 脚本状态，后接 `true` 为启用，`false` 为禁用
  
  - 小白理解：http-request 正则表达式 script-path=脚本路径,tag = 脚本名称,enable=脚本状态（写 `true` 为启用，`false` 为禁用）
  
- `http-response` 语句，示例：
```
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
```
  - `http-response` <===> 固定格式，表明语句类型
  
  - `^https?:\/\/(www.)?(example)\.com` <===> 正则表达式匹配到地址时执行脚本
  
  - `script-path=` <===> 固定格式，后接脚本路径
  
  - `https://example.com/loon.js` <===> 脚本路径
  
  - `timeout=` <===> 最大超时
  
  - `requires-body =` <===> 固定格式，是否包含Body，后接 `true` 为是，`false` 为否
  
  - `tag =` <===> 固定格式，意思为：标签，即用户将该语句自定义名称
  
  - `requestScript` <===> 脚本名称，按用户个人喜爱命名即可
  
  - `enable=` <===> 脚本状态，后接 `true` 为启用，`false` 为禁用
  
  - 小白理解：http-response 正则表达式 script-path=脚本路径,timeout=时间（单位为秒）,requires-body = 是否包含Body（写 `true` 为是，`false` 为否）,tag = 脚本名称,enable=脚本状态（写 `true` 为启用，`false` 为禁用）
  
- `cron` 语句，实例：
```
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true
```
  - `cron` <===> 固定格式，表明语句类型
  
  - `"0 8 * * *"` <===> cron 表达式，脚本执行时间，如果未了解 `cron 表达式` ，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md) 跳转到 `基础 cron 表达式的学习` 教程
  
  - `script-path=` <===> 固定格式，后接脚本路径
  
  - `tag =` <===> 固定格式，意思为：标签，即用户将该语句自定义名称
  
  - `requestScript` <===> 脚本名称，按用户个人喜爱命名即可
  
  - `enable=` <===> 启用状态，后接 `true` 为启用，`false` 为禁用
  
  - 小白理解：cron "cron 表达式" script-path=脚本路径,tag = 脚本名称,enable=脚本状态（写 `true` 为启用，`false` 为禁用）
