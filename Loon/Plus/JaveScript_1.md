# 入门

个人认为，每个新手用户在配置完 Loon 的基础设置后，都更多的希望能在 Loon 中添加脚本，利用脚本达到用户想要的效果，但是却不知道如何配置，此教程就让新手用户如何看懂一个脚本配置说明，并在下一个教程中讲述如何添加

## 脚本配置说明

目前整理出来的脚本开发者主要有以下几位，排名不分先后，这里将脚本开发者分成两类

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
