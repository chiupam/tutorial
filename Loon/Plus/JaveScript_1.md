# 入门

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 个人认为，每个新手用户在设置完 Loon 的基础设置后，都更多的希望能在 Loon 中添加脚本，利用脚本达到用户想要的效果，但是却不知道如何配置，此教程就让新手用户如何看懂一个脚本配置说明，并在下一个教程中讲述如何添加脚本

## 脚本

目前整理出来的脚本开发者主要有以下几位，排名不分先后，这里将脚本开发者分成四类

- 将脚本的配置方法写在 `脚本文件` 内的脚本开发者：

  - [lowking](https://github.com/lowking/Scripts/tree/master)（QQ会员签到）
  
  - [lowking](https://github.com/lowking/Scripts/tree/master)（开发者宣布仓库已不再维护）
  
  - [toulanboy](https://github.com/toulanboy/scripts/tree/master) 
  
  - [lxk0301](https://github.com/lxk0301/scripts)（京东系列小游戏）
  
  - [vinewx](https://ooxx.be/js) 
  
  - [Peng-YM](https://github.com/Peng-YM/QuanX/tree/master/Tasks)（彩云天气）
  
  - [NobyDa](https://github.com/NobyDa/Script/tree/master) （野比大神）
  
  - [evilbutcher](https://github.com/evilbutcher/Quantumult_X/tree/master) 
  
- 将脚本的配置方法写在 `REAMDE.md` 内的脚本开发者：

  - [chavyleung](https://github.com/chavyleung/scripts)（签到狂魔）
  
  - [zZpiglet](https://github.com/zZPiglet/Task)（滴滴打车）
  
  - [chouchoui](https://github.com/chouchoui/QuanX)
  
  - [yichahucha](https://github.com/yichahucha/surge)（历史价格）
  
- 有时将脚本的配置方法写在 `脚本文件` 内，又有时将脚本的配置方法写在 `REAMDE.md` 内的脚本开发者：

  - [chouchoui](https://github.com/chouchoui/QuanX) 
  
  - [saza34](https://github.com/sazs34/TaskConfig)（多合一签到脚本）
  
- 将各位开发者的脚本整合在一起的作者：

  - [nzw9314](https://github.com/nzw9314/QuantumultX/tree/master)（作者宣布于2020.08.09正式停止更新，在此之前已经收录的脚本能够正常使用）
  
  - [songyangzz](https://github.com/songyangzz/QxScripts) 
  
## 如何让 Loon 执行这些脚本

- 对于需要获取 `cookie` 类的签到脚本，例如：京东京豆签到脚本，需要

  - 在 Loon 配置文件中 `[Script]` 下添加以 `http-request` 和 `cron` 开头的语句，在 `[MITM]` 下的 `hostname = ` 后面添加域名
  
  - 按照脚本配置方法获取 `cookie`
  
  - 偶尔需要配合 `BoxJs` 使用
  
- 对于不需要获取 `cookie` 类的签到脚本，例如：京东小游戏系列脚本，需要

  - 在 Loon 配置文件中 `[Script]` 下添加以 `http-request` 和 `cron` 开头的语句，在 `[MITM]` 下的 `hostname = ` 后面添加域名
  
  - 偶尔需要配合 `BoxJs` 使用
  
- 对于仅提醒类，例如：nCov-19全球疫情通报脚本，需要

  - 在 Loon 配置文件中 `[Script]` 下添加以 `cron` 开头的语句
  
- 对于一些配置方法较为复杂的脚本，需要根据具体脚本内配置方法说明在 Loon 的配置文件中写入相关代码

## 对 `http-request` 、 `http-response` 以及 `cron` 语句格式的基本认识

- `http-request` 语句，示例：
```
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
```
  - http-request <===> 固定格式，表明语句类型
  
  - ^https?:\/\/(www.)?(example)\.com <===> 匹配访问地址的正则表达式
  
  - script-path= <===> 固定格式，后接脚本路径
  
  - localscript.js <===> 脚本路径
  
  - tag = <===> 固定格式，意思为：标签，即用户将该语句自定义名称
  
  - requestScript <===> 语句名称，按用户个人喜爱命名即可
  
  - enable= <===> 脚本状态，后接 `true` 为启用，`false` 为禁用
  
  - 小白理解：http-request 匹配访问地址的正则表达式 script-path=脚本路径,tag = 脚本名称,enable=脚本状态（脚本状态 `true` 为启用，`false` 为禁用）
  
- `http-request` 语句，示例：
```
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
```
  - http-request <===> 固定格式，表明语句类型
  
  - ^https?:\/\/(www.)?(example)\.com <===> 匹配访问地址的正则表达式
  
  - script-path= <===> 固定格式，后接脚本路径
  
  - localscript.js <===> 脚本路径
  
  - tag = <===> 固定格式，意思为：标签，即用户将该语句自定义名称
  
  - requestScript <===> 语句名称，按用户个人喜爱命名即可
  
  - enable= <===> 脚本状态，后接 `true` 为启用，`false` 为禁用
  
  - 小白理解：http-request 匹配访问地址的正则表达式 script-path=脚本路径,tag = 脚本名称,enable=脚本状态（脚本状态 `true` 为启用，`false` 为禁用）
  
- `cron` 语句，实例：
```
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true
```
  - cron <===> 固定格式，表明语句类型
  
  - "0 8 * * *" <===> cron 表达式，脚本执行时间，如果未了解 `cron 表达式` ，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md) 跳转到 `基础 cron 表达式的学习` 教程
  
  - script-path= <===> 固定格式，后接脚本路径
  
  - tag = <===> 固定格式，意思为：标签，即用户将该语句自定义名称
  
  - requestScript <===> 语句名称，按用户个人喜爱命名即可
  
  - enable= <===> 启用状态，后接 `true` 为启用，`false` 为禁用
  
  - 小白理解：cron "cron 表达式" script-path=脚本路径,tag = 脚本名称,enable=脚本状态（脚本状态 `true` 为启用，`false` 为禁用）

## 初步了解脚本文件内使用说明和配置

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 以京东京豆签到脚本为例，该脚本为 NobyDa(野比) 开发，由于脚本配置说明写在脚本文件内，所以首先打开脚本文件

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 Raw ，此步为重要的一步，脚本配置说明写在脚本文件内的，都需要点击 Raw 后查看

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 阅读脚本文件开头说明，寻找与 `Loon配置` 等相关字眼，明晰 Loon 内配置文件该如何写入语句

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 寻找与 `使用说明` 等相关字眼，方便后续操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_4.jpg)

# 多说几句

- 阅读完此教程后，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_2.md) 跳转到 `初级 —— 如何将脚本配置写入 Loon 内发挥作用` 教程，正式进入 Loon 配置文件内相关位置写入脚本配置的相关代码

# 鸣谢

- [NobyDa](https://github.com/NobyDa)
