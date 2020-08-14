# cron 表达式

通过对 cron 表达式的修改，定时执行脚本

## 一、学习 cron 表达式的基本写法

\*    \*    \*    \*    \*

\-    \-    \-    \-    \-
|    |    |    |    |
|    |    |    |    +----- 星期几 (0 - 7) 或者 SUN,MON,TUE,WED,THU,FRI,SAT
|    |    |    +---------- 月份 (1 - 12) 或者 JAN,FEB,MAR,APR ...
|    |    +--------------- 日期 (1 - 31)
|    +-------------------- 时 (0 - 23)

+------------------------- 分 (0 - 59)

## 一、修改本地脚本中的 cron 表达式

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方 `配置` 栏，下拉找到并点击 `本地脚本`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Local_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到需要修改 cron 表达式的脚本并点击（左下角如果不是 `cron` 的不能修改）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `表达式` 右侧并按用户需要修改

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_5.jpg)

- 5 0 * * * 表示 每日 12：05 执行一次

- 学习更多 cron 语法，请点击 [这里](https://tool.lu/crontab/)
