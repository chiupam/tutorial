# 添加本地路径脚本

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 此教程让用户通过对 Loon 的 UI 操作，在 Loon 内添加一个引用路径为**本地路径**的脚本

## 从 URL 下载脚本文件到 icloud/Loon/Script

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) 跳转到 `添加脚本文件 - 从URL下载` 教程

## 充分理解脚本文件内配置代码

**以京东京豆签到脚本为例**

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 阅读脚本文件内的配置代码，如下图区域 `[Script]` 下的 `http-request` 代码所示

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JD-DailyBonus_http-request.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 按照三种脚本语句格式拆解这段配置代码，**明晰哪些地方可以自行修改，哪些地方不可自行修改**

**如果用户对三种脚本语句格式不了解，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format.md) 跳转到 `入门 —— 如何看懂三种脚本语句的必备格式` 教程**

- 用户不可自行修改的项目与填写位置

  - `http-request` <===> 脚本类型

  - ` https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean` <===> 表达式

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

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择 `Local`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `脚本名称`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_8.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择通过 `从 URL 下载` 功能下载而来的 `JD_DailyBonus.js` 文件

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 正确的写法如下图所示，确定无误后点击 `保存` 即可完成操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_10.jpg)

# 多说几句

- Loon 是开放远程脚本链接的，如果用户不需要修改脚本文件内代码，极力推荐学习 `添加远程链接脚本` 教程以及使用 `添加远程链接脚本` 功能，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_JaveScript.md) 跳转到 `添加远程链接脚本` 教程

- 再次强调，此教程的前提是需要用户提前通过 `从URL下载` 功能将脚本下载到 icloud/Loon/Script 文件夹内并在 Loon 开启 `自动同步` 功能，如果用户还没有进行操作此步，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) 跳转到 `添加脚本文件 - 从URL下载` 教程


