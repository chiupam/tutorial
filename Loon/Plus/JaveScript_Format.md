# 对 Loon 脚本语句格式的基本认识

Loon 目前的脚本语句只有三种，即 `http-request` 、 `http-response` 以及 `cron` 语句，小白理解了这三种语句，对于通过 UI 添加脚本或者直接在 Loon 内配置写入脚本语句都有极大的提高

- TF 2.1.13(199) 更新：新增network-changed类型脚本，会在网络环境发生变化是触发脚本，增加获取配置以及设置策略、运行模式脚本API

## `http-request` 语句

示例：

```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
```

拆解：

 - `http-request` <===> 固定格式，不可修改，表明语句类型
  
 - `^https?:\/\/(www.)?(example)\.com` <===> 正则表达式匹配到地址时执行脚本，不可修改
  
 - `script-path=` <===> 固定格式，不可修改，后接脚本路径
  
 - `localscript.js` <===> 脚本路径，远程链接时推荐不要修改，本地位置时根据实际情况选择脚本
  
 - `tag =` <===> 固定格式，不可修改，意思为：标签，即用户将该语句自定义名称
  
 - `requestScript` <===> 脚本名称，可修改，按用户个人喜爱命名即可
  
 - `enable=` <===> 脚本状态，可修改，按照用户需求自行修改， `=` 后接 `true` 为启用，`false` 为禁用
  
 理解：
 
 http-request 正则表达式 script-path=脚本路径,tag = 脚本名称,enable=脚本状态（写 `true` 为启用，`false` 为禁用）
  
## `http-response` 语句

示例：

```
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
```

拆解：

 - `http-response` <===> 固定格式，不可修改，表明语句类型
 
 - `^https?:\/\/(www.)?(example)\.com` <===> 正则表达式匹配到地址时执行脚本，不可修改

 - `script-path=` <===> 固定格式，不可修改，后接脚本路径
 
 - `https://example.com/loon.js` <===> 脚本路径
  
 - `timeout=` <===> 最大超时
  
 - `requires-body =` <===> 固定格式，不可修改，是否包含Body，后接 `true` 为是，`false` 为否
  
 - `tag =` <===> 固定格式，不可修改，意思为：标签，即用户将该语句自定义名称
  
 - `requestScript` <===> 脚本名称，按用户个人喜爱命名即可
  
 - `enable=` <===> 脚本状态，按照用户需求自行修改， `=` 后接 `true` 为启用，`false` 为禁用
  
小白理解：

http-response 正则表达式 script-path=脚本路径,timeout=时间（单位为秒）,requires-body = 是否包含Body（写 `true` 为是，`false` 为否）,tag = 脚本名称,enable=脚本状态（写 `true` 为启用，`false` 为禁用）
  
## `cron` 语句

实例：

```
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true
```

拆解：

 - `cron` <===> 固定格式，不可修改，表明语句类型
  
 - `"0 8 * * *"` <===> cron 表达式，脚本执行时间，根据用户需求自行修改，如果未了解 `cron 表达式` ，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md) 跳转到 `基础 cron 表达式的学习` 教程
  
 - `script-path=` <===> 固定格式，不可修改，后接脚本路径
  
 - `tag =` <===> 固定格式，不可修改，意思为：标签，即用户将该语句自定义名称
  
 - `requestScript` <===> 脚本名称，按用户个人喜爱命名即可
  
 - `enable=` <===> 启用状态，按照用户需求自行修改， `=` 后接 `true` 为启用，`false` 为禁用
  
小白理解：

cron "cron 表达式" script-path=脚本路径,tag = 脚本名称,enable=脚本状态（写 `true` 为启用，`false` 为禁用）


## `network-changed` 语句

实例：

```
network-changed script-path=https://raw.githubusercontent.com/Loon0x00/LoonExampleConfig/master/Script/netChanged.js, tag=changeModel,enable=true
```

拆解：

 - `network-changed` <===> 固定格式，不可修改，表明语句类型
  
 - `script-path=` <===> 固定格式，不可修改，后接脚本路径
  
 - `tag =` <===> 固定格式，不可修改，意思为：标签，即用户将该语句自定义名称
  
 - `enable=` <===> 启用状态，按照用户需求自行修改， `=` 后接 `true` 为启用，`false` 为禁用
  
小白理解：

network-changed script-path=脚本路径, tag=脚本名称,enable=脚本状态（写 `true` 为启用，`false` 为禁用）