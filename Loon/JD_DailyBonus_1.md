# 京东京豆签到脚本配置方法

通过学习如何配置京东京豆签到脚本，学会如何在 Loon 中配置内写入一个签到脚本

## 在 Loon 中添加脚本的配置步骤主要有两个

- 1、需要配置 [Script] 代码片段，或在UI界面输入，但此教程在这里只教最原始的——本地编辑配置

- 2、需要配置 [Mitm] 下的 hostname 域名，或直接通过 Loon 配置栏-MITM-域名 添加，但此教程在这里也只教最原始的——本地编辑配置

## 第一种方法(请必须先用第一种方法再学习后面的方法)

### 一、查看脚本文件

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 请点击 [这里](https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js) 跳转到 safari 中直到配置完成

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_1.jpg)

### 二、进入 Loon 进行编辑配置

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方配置栏

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/bianji.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 以下几步会在 safari 与 Loon 之间切换进行操作复制粘贴代码片段的操作，先进入[刚才在 safari 打开的网页](https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js)拷贝如下图所示的代码片段

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将上图拷贝下来的代码片段粘贴到下图指定位置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 继续回到 safari 中拷贝如下图所示的代码片段

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_hostname.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将上图拷贝下来的代码片段粘贴到下图指定位置，完成后点右上角保存按钮保存，注意：hostname 每两个地址的间隔方法：前一个地址与后一个地址用一个英文逗号隔开)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/hostname.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 正确的配置如下图所示

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_2.jpg)

### 三、完成上述配置后 请回到 safari 中

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 拷贝如下图所示的网址，或者点击 [这里]() 跳转

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 safari 粘贴并前往获取 cookie 的网址，点击箭头所指区域

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_safari_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 最后会弹窗提示获取 cookie 成功，如果没有弹窗，请往下看

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_safari_2.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如果没有提示可能原因是：

- 没有正确配置

- 曾经已经成功获取（需要重新获取 cookie 请深入学习 BoxJs 的使用方法并订阅 NobyDa 的 BoxJs）

## 四、对脚本执行时间进行修改(此步是按需操作)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方配置栏

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Local_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击此处

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 按需要修改，如果不懂 cron 语法，请点击 [这里](https://tool.lu/crontab/)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_5.jpg)

- 5 0 * * * 表示 每日 12：05 执行一次

- 学习更多 cron 语法，请点击 [这里](https://tool.lu/crontab/)

## 第二种方法与第三种方法

这两种方法都比较类似，我将它们写在另一个文档内，请点击 [这里](https://github.com/Dadong111/tutorial/blob/master/JD_DailyBonus_2%263.md)

# 鸣谢

- [NobyDa](https://github.com/NobyDa)    

- 以及 NobyDa 的[京东京豆签到脚本](https://github.com/NobyDa/Script/blob/master/JD-DailyBonus/JD_DailyBonus.js)
