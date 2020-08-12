# 一、进入 Surge 进行 [MITM] 相关配置(此处并未包含执行脚本的配置)：

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先在 safari 中打开右侧这串地址：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 再进行下面的操作

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Suege 并点击左上角所示区域

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/peizhi.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 在文本模式中编辑（如果没有则点击 创建当前配置副本 点击 好的 再进行操作）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/bianji.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 返回 safari 找到并复制/拷贝如图所示的代码片段

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/caiyun_hostname.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 粘贴到如图所示的指定位置 [MITM] 下的 hostname = 后面并点击右上角完成，注意：添加 hostname 的时候，每个地址之间用英文逗号加空格间隔

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/hostname.jpg)

# 二、进入 Surge 脚本卡片添加 http-request 和 cron： 

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Surge 并点击脚本卡片中的脚本按钮

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/Script_local.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击新增

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/Script_new.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 按图填写内容，URL 正则表达式和脚本URL 都在教程下面，请自行复制粘贴，填写完成后点击右上角完成按钮

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/caiyun_request.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将脚本类型由 HTTP Request 更改为 Cron 后，再将脚本位置由 本地 更改为 远程，最后按图填写内容，cron 表达式和脚本 URL 都在教程下面，请自行复制粘贴，填写完成后点击右上角完成按钮

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Surge/caiyun_cron.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) URL 正则表达式：https:\/\/((weather-data\.apple)|(api.weather))\.com

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) cron表达式：0 7-22/3 * * * (意思为 每天7-22点每3小时的第0分执行一次脚本，即7点、10点、13点，以此类推)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 脚本 URL：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 
