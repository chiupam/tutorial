# Basic understanding of Loon script statement format

Loon currently has only three kinds of script statements, namely `http-request`, `http-response` and `cron` statements. Popular understanding these three statements. For adding scripts through the UI or directly configuring and writing scripts in Loon The sentences have been greatly improved

- TF 2.1.13(199) update: Added network-changed type scripts, which will trigger scripts when the network environment changes, and add access to configuration and setting strategies, operating mode script APIs

## `http-request` statement

Example:

```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
```

Dismantling:

 - `http-request` <===> fixed format, cannot be modified, indicating the type of statement
  
 - `^https?:\/\/(www.)?(example)\.com` <===> Execute the script when the regular expression matches the address, and cannot be modified
  
 - `script-path=` <===> Fixed format, cannot be modified, followed by script path
  
 - `localscript.js` <===> script path, it is recommended not to modify it during remote linking, select the script according to the actual situation in the local location
  
 - `tag =` <===> Fixed format, cannot be modified, meaning: tag, that is, the user defines the name of the sentence
  
 - `requestScript` <===> Script name, which can be modified, just name it according to user's preference
  
 - `Enable=` <===> Script status, which can be modified and modified according to user needs, `=` followed by `true` to enable, and `false` to disable
  
 understanding:
 
 http-request regular expression script-path=script path,tag=script name,enable=script status (write `true` to enable, `false` to disable)
  
## `http-response` statement

Example:

```
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
```

Dismantling:

 -`http-response` <===> fixed format, cannot be modified, indicating the type of statement
 
 -`^https?:\/\/(www.)?(example)\.com` <===> Execute the script when the regular expression matches the address, and cannot be modified

 -`script-path=` <===> Fixed format, cannot be modified, followed by script path
 
 -`https://example.com/loon.js` <===> script path
  
 -`timeout=` <===> Maximum timeout
  
 -`requires-body =` <===> Fixed format, unmodifiable, whether to include Body, followed by `true` for yes, `false` for no
  
 -`tag =` <===> Fixed format, cannot be modified, meaning: tag, that is, the user defines the name of the sentence
  
 -`requestScript` <===> script name, just name it according to the user's personal preference
  
 -ʻEnable=` <===> Script status, modify according to user needs, `=` followed by `true` to enable, and `false` to disable
  
Popular understanding:

http-response regular expression script-path= script path, timeout= time (in seconds), requires-body = whether to include Body (write `true` for yes, `false` for no), tag = script name, enable =Script status (write `true` to enable, `false` to disable)
  
## `cron` statement

Examples:

```
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true
```

Dismantling:

 - `cron` <===> fixed format, cannot be modified, indicating the type of statement
  
 - `"0 8 * * *"` <===> cron expression, script execution time, modify according to user needs, if you don’t know `cron expression`, please click [here](https://github. com/chiupam/tutorial/blob/master/Loon/Plus/cron.md) Jump to the `Basic cron expression learning` tutorial
  
 - `script-path=` <===> Fixed format, cannot be modified, followed by script path
  
 - `tag =` <===> Fixed format, cannot be modified, meaning: tag, that is, the user defines the name of the sentence
  
 - `requestScript` <===> script name, just name it according to the user's personal preference
  
 - ʻEnable=` <===> Enable state, modify according to user needs, `=` followed by `true` to enable, and `false` to disable
  
Popular understanding:

cron "cron expression" script-path=script path,tag=script name,enable=script status (write `true` to enable, `false` to disable)


## `network-changed` statement

Examples:

```
network-changed script-path=https://raw.githubusercontent.com/Loon0x00/LoonExampleConfig/master/Script/netChanged.js, tag=changeModel,enable=true
```

Dismantling:

 - `network-changed` <===> fixed format, cannot be modified, indicating the type of statement
  
 - `script-path=` <===> Fixed format, cannot be modified, followed by script path
  
 - `tag =` <===> Fixed format, cannot be modified, meaning: tag, that is, the user defines the name of the sentence
  
 - ʻEnable=` <===> Enable state, modify according to user needs, `=` followed by `true` to enable, and `false` to disable
  
Popular understanding:

network-changed script-path= script path, tag= script name, enable= script status (write `true` to enable, `false` to disable)