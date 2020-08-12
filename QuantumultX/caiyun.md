# [caiyun.js](https://github.com/Peng-YM/QuanX/blob/master/Tasks/caiyun.js) 来自 [Peng-YM](https://github.com/Peng-YM) 大佬的 [github 库](https://github.com/Peng-YM/QuanX/tree/master/Tasks)

### 功能：

√ 自动定位
√ 异常天气预警
√ 实时天气预报
√ 降雨提醒
√ 每日睡前预报

## 一、申请彩云天气令牌：(审核通过需要2-3天，留意注册邮箱)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先打开右侧这串地址：https://dashboard.caiyunapp.com/user/sign_up/

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_1.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_2.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_3.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_4.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_5.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_6.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_7.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_8.png)

## 二、申请腾讯地图令牌：(正确填入申请信息可立马通过审核)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先打开右侧这串地址：https://lbs.qq.com/dev/console/user/info

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_1.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_2.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_3.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_4.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_5.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_6.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_7.png)

## 三、进入 BoxJS (如果是第一次使用 BoxJS 请点击 [这里](https://github.com/chiupam/tutorial/blob/master/QuantumultX/BoxJS.md) 并完成教程中第一步的配置)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先复制右侧这串地址：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/box.js.json

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 safari 并进入 [BoxJS](http://boxjs.com) 设置界面 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_2.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_3.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_4.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_5.png)

## 四、进入 QX 进行 [rewrite_local] 与 [mitm] 相关配置(此处并未包含 [task] 的配置)：

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先打开右侧这串地址：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 再进行下面的操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/dianji.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/bianji.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_rewrite.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/rewrite_local.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_hostname.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 添加 hostname 的时候，每个地址之间用英文逗号加空格间隔

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/hostname.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/changan.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/up.png)

### QX 内正确配置应该如下图所示

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_right.png)

## 五、进入 iOS 自带的天气 app 自动获取当前定位(会有弹窗提醒)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开手机设置 > 隐私 > 定位服务

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开定位服务

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 选择天气，选择使用 APP 期间

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 此时，打开系统天气应用，会提示获取位置成功，如果没有提示，请确认上面的步骤是否配置正确

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 请确保自己手机内的天气 APP 中只有一个城市的天气预报

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_weatherapp.png)

## 六、进入 QX 配置 [task] 即添加任务请求

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/task_ui.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_1.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_2.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_3.png)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_4.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) cron表达式：0 7-22/3 * * * (意思为 每天7-22点每3小时的第0分执行一次脚本，即7点、10点、13点，以此类推)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 脚本路径：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 图标：https://raw.githubusercontent.com/Orz-3/task/master/caiyun.png 来自 [Orz-3 契阔大佬](https://github.com/Orz-3/task)

### 此处的正确写法

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_5.png)

# 鸣谢

- Peng-YM [github库](https://github.com/Peng-YM) 提供的 caiyun.js 脚本

- Orz-3 [github库](https://github.com/Orz-3) 提供的图标 [TG频道](https://t.me/Orzmini)
