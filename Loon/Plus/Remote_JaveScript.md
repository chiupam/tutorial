# 添加远程链接脚本

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 此教程让用户通过对 Loon 的 UI 操作，在 Loon 内添加一个引用路径为**远程路径**的脚本

## 充分理解脚本文件内配置代码

**以京东京豆签到脚本为例**

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 阅读脚本文件内的配置代码，如下图区域 `[Script]` 下的 `http-request` 代码所示

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JD-DailyBonus_http-request.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 按照三种脚本语句格式拆解这段配置代码，**明晰哪些地方可以自行修改，哪些地方不可自行修改**

**如果用户对三种脚本语句格式不了解，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format.md) 跳转到 `入门 —— 如何看懂三种脚本语句的必备格式` 教程**

- 用户不可自行修改的项目与填写位置

  - `http-request` <===> 脚本类型

  - ` https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean` <===> 表达式
  
  - `https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js` <===> 脚本远程链接

- 用户可自行修改的项目与填写位置

  - `获取京东cookie` <===> 别名

## 通过 UI 添加脚本

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `添加脚本`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击如图所示区域（+）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_1.jpg)

**以添加 http-request 语句为例**

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `脚本类型`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择 `http-request`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `别名` 栏写入脚本名称，按用户个人喜爱，自行命名，最好以脚本功能命名

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `表达式` 栏写入匹配网址执行脚本的正则表达式，即 ` https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `脚本位置`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择 `Remote`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_7_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在 `脚本链接` 栏写入脚本远程链接，即 `https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_8_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 正确的写法如下图所示，确定无误后点击 `保存` 即可完成操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_10_2.jpg)
