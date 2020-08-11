# 京东京豆签到脚本配置方法

- 此方法比较简单粗暴，必须先学习第一种方法再来学习该方法

- 如果浏览者未学习第一种方法，请点击 [这里]()

## 第二种方法（通过订阅脚本功能）

### 一、进入 Loon 订阅脚本

先复制右侧这串地址：https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/JD_DailyBonus.conf

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Script.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Script_1.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Script_2.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_remote_1.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_remote_2.jpg)

### 二、完成上述配置后 请回到 safari 中获取 cookie

- Safari浏览器打开登录 https://bean.m.jd.com ,点击签到并且出现签到日历后, 如果通知获得cookie成功, 则可以使用此签到脚本。

- 也可以回到第一种方法种查看操作步骤（三）

### 二、对脚本执行时间进行修改(此步是按需操作)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_remote_3.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_remote_4.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_remote_5.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_remote_6.jpg)

## 第三种方法（通过插件功能）

### 一、进入 Loon 订阅插件

先复制右侧这串地址：https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/JD_DailyBonus.plugin

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plugin.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plugin_1.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_plugin_1.jpg)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/JD_DailyBonus_plugin_2.jpg)

### 二、完成上述配置后 请回到 safari 中获取 cookie

- Safari浏览器打开登录 https://bean.m.jd.com ,点击签到并且出现签到日历后, 如果通知获得cookie成功, 则可以使用此签到脚本。

- 也可以回到第一种方法种查看操作步骤（三）

## 这两种方法的区别

- 第二种方法优先级比第三种方法的低

- 第二种方法可以修改执行时间，即可以修改 cron 表达式，第三种则不行，需要引用到的地址的作者在其库中修改

- 感兴趣可以学习如何写 .plugin 文件放在个人 github 库中，在插件中引用个人链接，高度自定义
