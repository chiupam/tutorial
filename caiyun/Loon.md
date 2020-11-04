# 一、进入 Loon 进行 [Script] 与 [MITM] 相关配置

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先在 safari 中打开右侧这串地址：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 再进行下面的操作

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方配置栏，下拉，点击文本编辑

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/unknow/bianji.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 返回 safari 找到并复制/拷贝如图所示的代码片段

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/unknow/caiyun_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 粘贴到如图所示的指定位置 [Script] 下面

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/unknow/Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 返回 safari 找到并复制/拷贝如图所示的代码片段

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/unknow/caiyun_hostname.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 粘贴到如图所示的执行位置 [mitm] 下的 hostname = 后面并点击右上角保存，注意：添加 hostname 的时候，每个地址之间用英文逗号加空格间隔

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/unknow/hostname.jpg)

# 二、进入 Loon 本地脚本内进行相关配置

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方配置栏，下拉，点击本地脚本

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/unknow/Local_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将脚本类型由 http-request 更改为 cron 后，按下图配置，cron 表达式与脚本链接放在下面，自行复制粘贴

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/unknow/caiyun_local_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) cron表达式：0 7-22/3 * * * (意思为 每天7-22点每3小时的第0分执行一次脚本，即7点、10点、13点，以此类推)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 脚本链接：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 
