# 添加本地路径脚本

**此教程的前提是需要用户提前通过 `从URL下载` 功能将脚本下载到 icloud/Loon/Script 文件夹内，如果用户还没有进行操作此步，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) 跳转到 `添加脚本文件 - 从URL下载` 教程**

此教程让用户通过对 Loon 的 UI 操作，在 Loon 内添加一个引用路径为**本地路径**的脚本

## 从 URL 下载脚本文件到 icloud/Loon/Script

请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) 跳转到 `添加脚本文件 - 从URL下载` 教程

## 充分理解脚本文件内配置代码

**以京东京豆签到脚本为例**

阅读配置代码，如下图区域代码所示

按照三种脚本语句格式拆解配置代码，为下一步操作做准备

**如果用户对三种脚本语句格式不了解，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format.md) 跳转到 `入门 —— 如何看懂三种脚本语句的必备格式` 教程**

## 通过 UI 添加脚本

打开 Loon 并点击下方 `配置` 栏，点击 `添加脚本`

点击如图所示区域（+）

**以添加 http-request 语句为例**

点击 `脚本类型`

选择 `http-request`

在 `别名` 栏写入脚本名称，按用户个人喜爱，自行命名，最好以脚本功能命名

在 `表达式` 栏写入匹配网址执行脚本的正则表达式，即 ` https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean`

点击 `脚本位置`

选择 `Local`

点击 `脚本名称`

选择 `从 URL 下载` 的 `JD_DailyBonus.js` 文件

正确的写法如下图所示，确定无误后点击 `保存` 即可完成操作

# 多说几句

- Loon 是开放远程脚本链接的，如果用户不需要修改脚本文件内代码，极力推荐学习 `添加远程链接脚本` 教程以及使用 `添加远程链接脚本` 功能，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_JaveScript.md) 跳转到 `添加远程链接脚本` 教程

- 再次强调，此教程的前提是需要用户提前通过 `从URL下载` 功能将脚本下载到 icloud/Loon/Script 文件夹内并在 Loon 开启 `自动同步` 功能，如果用户还没有进行操作此步，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) 跳转到 `添加脚本文件 - 从URL下载` 教程


