# cron 表达式

通过对 cron 表达式的修改，定时执行脚本

## 一、学习 cron 表达式的基本写法

1、cron 6位表达式

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/cron_6.png)

- 从左到右依次

  - 第一位代表 `秒` ，只允许写 `0-59` 之间的数字
  
  - 第二位代表 `分` ，只允许写 `0-59` 之间的数字，不允许出现 `60`
  
  - 第三位代表 `时` ,只允许写 `0-23` 之间的数字，凌晨12时不允许写 `24`
  
  - 第四位代表 `日` ，只允许写 `1-31` 之间的数字
  
  - 第五位代表 `月` ，只允许写 `1-12` 之间的数字
  
  - 第六位代表 `星期` ，只允许写 `0-7` 之间的数字， `0` 和 `7` 都代表周日
  
2、cron 5位表达式

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/cron_5.png)

- 从左到右依次
  
  - 第一位代表 `分` ，只允许写 `0-59` 之间的数字，不允许出现 `60`
  
  - 第二位代表 `时` ,只允许写 `0-23` 之间的数字，凌晨12点时不允许写 `24`
  
  - 第三位代表 `日` ，只允许写 `1-31` 之间的数字
  
  - 第四位代表 `月` ，只允许写 `1-12` 之间的数字
  
  - 第五位代表 `星期` ，只允许写 `0-7` 之间的数字， `0` 和 `7` 都代表周日
  
3、特殊字符

- `*` 代表任何值，如 `* * * * *` 代表 `每分钟执行一次`

- `/` 代表每，如 `10-20/5 * * * *` 代表 `每小时里的10-20分，每5分钟执行一次`

- 

## 二、修改本地脚本中的 cron 表达式

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方 `配置` 栏，下拉找到并点击 `本地脚本`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Local_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到需要修改 cron 表达式的脚本并点击（左下角如果不是 `cron` 的不能修改）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `表达式` 右侧并按用户需要修改

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_local_5.jpg)

- 5 0 * * * 表示 每日 12：05 执行一次

- 学习更多 cron 语法，请点击 [这里](https://tool.lu/crontab/)
