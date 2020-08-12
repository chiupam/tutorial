# 一、进入 QX 进行 [rewrite_local] 与 [mitm] 相关配置(此处并未包含 [task] 的配置)：

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先打开右侧这串地址：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 再进行下面的操作

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击小风车

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/dianji.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 下拉，点击编辑

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/bianji.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 返回 safari 找到并复制/拷贝如图所示的代码片段

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_rewrite.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 粘贴到如图所示的指定位置 [rewrite_local] 下面

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/rewrite_local.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 返回 safari 找到并复制/拷贝如图所示的代码片段

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_hostname.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 粘贴到如图所示的执行位置 [mitm] 下的 hostname = 后面并点击右上角保存，注意：添加 hostname 的时候，每个地址之间用英文逗号加空格间隔

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/hostname.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 回到此界面，长按小风车

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/changan.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击左侧灰色按钮，一键更新外部资源（购买未满30天用户无法使用此方法缓存脚本）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/up.png)

# 二、进入 QX 配置 [task] 即添加任务请求

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击小风车

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/dianji.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 下拉找到构造请求并点击

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/task_ui.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击右上角 + 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_1.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击高级

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_2.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如图所示按要求填写，远链放在下面，自行复制粘贴，完成后点击右上角确定

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_3.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击全部更新

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_4.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) cron表达式：0 7-22/3 * * * (意思为 每天7-22点每3小时的第0分执行一次脚本，即7点、10点、13点，以此类推)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 脚本路径：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 图标：https://raw.githubusercontent.com/Orz-3/task/master/caiyun.png 来自 [Orz-3 契阔大佬](https://github.com/Orz-3/task)
