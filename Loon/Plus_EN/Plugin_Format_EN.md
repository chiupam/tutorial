# Add plugin URL

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) This tutorial allows users to learn about the format requirements and content requirements of the URL filled in in the `add plugin`

## 1. Requirements for URL format and content

-Requirements for URL format

  -For files uploaded to the github library, the subscription address URL must start with `http://raw`
  
-Requirements for URL content

  -Must have a Loon configuration file format, currently supports `[Rule]`, `[URL Rewrite]`, `[Script]`, `[MITM]` modules for the time being, and more modules will be expanded later
  
## 2. URL content demonstration

```
[Rule]
DOMAIN,google.com,PROXY

[URL Rewrite]
^https?:\/\/(www.)?(g|google)\.cn https://www.google.com 302

[Script]
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true

[MITM]
hostname = *.example.com,*.sample.com
```

## Three. URL example file demonstration

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click directly on the address below to view the correct format of the URL content

https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/Plugin_Example.conf

## Fourth, the method to obtain the correct URL link

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the file that needs to subscribe to the script

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Plugin_Raw_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click Raw

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Plugin_Raw_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Long press the address bar and click `copy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Plugin_Raw_3.jpg)

# Say a few more words

-Although the `[Script]` module is supported, it is not recommended to write the script configuration code of the **check-in script** into the plug-in file, because adding scripts in this way does not allow users to modify the script execution time

-It is recommended to write script configuration code similar to `Jingdong, Taobao historical price script` into the plug-in file, because such scripts will not have pop-up reminders, and there is no need to modify the execution time