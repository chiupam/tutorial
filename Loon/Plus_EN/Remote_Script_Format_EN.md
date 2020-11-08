# Subscription script URL

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) This tutorial allows users to learn about the format requirements and content requirements of the URL filled in in the `subscription script`

## 1. Requirements for URL format and content

-Requirements for URL format

  -For files uploaded to the github library, the subscription address URL must start with `http://raw`
  
-Requirements for URL content

  -Must contain one or more script statements
  
  -You can write statements with `hostname =`
  
## 2. URL content demonstration

```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true

hostname = example1.com,example2.com
```

## Three. URL example file demonstration

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click directly on the address below to view the correct format of the URL content

https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/Remote_Script_Example.conf

## Fourth, the method to obtain the correct URL link

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the file that needs to subscribe to the script

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click Raw

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Long press the address bar and click `copy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Script_Raw_3.jpg)