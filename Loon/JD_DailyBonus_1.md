# 京东京豆签到脚本配置方法

通过学习如何配置京东京豆签到脚本，学会如何在 Loon 中配置内写入一个签到脚本

## 第一种方法(请必须先用第一种方法再学习后面的方法)

### 一、查看脚本文件

请点击 [这里](https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js) 跳转到 safari 中直到配置完成

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_1.jpg)

### 二、进入 Loon 进行编辑配置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/bianji.jpg)

safari 与 Loon 之间切换进行操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_script.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Script.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_hostname.jpg)

hostname 每两个地址的间隔方法：前一个地址与后一个地址用一个英文逗号隔开

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/hostname.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_2.png)

右上角保存即可

### 三、完成上述配置后 请回到 safari 中

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_3.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_safari_1.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_safari_2.jpg)

最后一张图片时会弹窗提示获取 cookie 成功，如果没有提示可能原因是：

- 没有正确配置

- 曾经已经成功获取（需要重新获取 cookie 请学习 BoxJs 的使用方法并订阅 NobyDa 的 BoxJs）

## 四、对脚本执行时间进行修改(此步是按需操作)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Local_Script.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_4.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_5.jpg)

- 5 0 * * * 表示 每日 12：05 执行一次

- 学习更多 cron 语法，请点击 [这里](https://tool.lu/crontab/)

## 第二种方法与第三种方法

这两种方法都比较类似，我将它们写在另一个文档内，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/JD_DailyBonus_2&3.md)
