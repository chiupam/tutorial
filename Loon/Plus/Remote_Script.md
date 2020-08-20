# 订阅脚本

订阅脚本通过读取 URL 内容，自动识别脚本语句和 hostname ，批量在 Loon 内添加脚本

## 对 URL 格式及内容的要求

- 对 URL 格式的要求

  - 文件上传至github库的 URL 必须以 `http://raw` 开头的网址
  
- 对 URL 内容的要求

  - 必须包含一条以上脚本语句
  
  - 可以写有 `hostname =` 的语句
  
## URL 内容示范

```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true

hostname = example1.com,example2.com
```
