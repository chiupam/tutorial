# 证书类问题

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如果运行 Loon 的过程中弹窗出现任何关于 **证书** 相关字眼的提醒，都请按下步骤检查

## 自检证书是否一致的方法

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `证书管理`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 记录如下图所示区域中显示的数字，记为 `1号证书`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开手机 **设置** >>> **通用** >>> **关于本机** >>> **证书信任设置**（此步骤不截图是因为懒癌发作，ios 13 系统以上都可以按照此步骤找到入口）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 记录如下图所示区域中显示的数字，记为 `2号证书`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 对比 `1号证书` 和 `2号证书` 是否一致

- 一致时但下方显示 `已安装，但未被系统信任` 时，请继续下列教程操作**信任证书**
Certificate_4
- 不一致时请继续按下列教程操作**重新安装证书**

## 信任证书

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开手机 **设置** >>> **通用** >>> **关于本机** >>> **证书信任设置**（此步骤不截图是因为懒癌发作，ios 13 系统以上都可以按照此步骤找到入口）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到与用户的 `1号证书` 数字相同的证书，点击右侧按钮使 `灰色按钮` 变成`绿色按钮` 即可完成**信任证书**操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_8.jpg)

## 重新安装证书

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开手机 **设置** >>> **通用** >>> **描述文件** >>> **LOON CA 2号证书的数字**（此步骤不截图是因为懒癌发作，ios 13 系统以上都可以按照此步骤找到入口）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `移除描述文件` 并输入密码

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `移除` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 然后打开 Loon 并点击下方 `配置` 栏，点击 `证书管理`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_UI.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `生成新的CA证书`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `安装CA证书`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在跳转出来的页面中点击 `允许`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开手机设置并点击 `已下载描述文件`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `安装` 后，出现验证的步骤，请用户自行输入密码验证

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 回到手机设置并点击 `通用` ，然后点击 `关于本机`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `证书信任设置`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击按钮使 `灰色按钮` 变成`绿色按钮` 即可完成操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_8.jpg)

多说几句

- 证书后的数字很重要，用户需要看准确，以及是否出现 `已安装，但未被系统信任` 的字样。以确定用户需要进行**重新安装证书**抑或是**信任证书**的操作
