# [caiyun.js](https://github.com/Peng-YM/QuanX/blob/master/Tasks/caiyun.js) 来自 [Peng-YM](https://github.com/Peng-YM) 大神的 github 库

### 功能：

√ 自动定位
√ 异常天气预警
√ 实时天气预报
√ 降雨提醒
√ 每日睡前预报

## 一、申请彩云天气令牌：

### 先打开下面这串地址：

https://dashboard.caiyunapp.com/user/sign_up/

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_1.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_2.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_3.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_4.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_5.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_6.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_7.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_api_8.png)

## 二、申请腾讯地图令牌：

### 先打开下面这串地址：

https://lbs.qq.com/dev/console/user/info

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_1.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_2.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_3.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_4.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_5.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_6.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/tencent_api_7.png)

## 三、进入 BoxJS (如果是第一次使用 BoxJS 请点击 [这里](https://github.com/chiupam/tutorial/blob/master/QuantumultX/BoxJS.md) 配置)

### 先复制下面这串地址：

https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/box.js.json

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_1.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_2.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_3.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_4.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_boxjs_5.png)

## 四、进入 QX 进行 [rewrite_local] 与 [mitm] 相关配置(此处并未包含 [task] 的配置)：

先打开右侧这串地址：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 再进行下面的操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/dianji.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/bianji.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/rewrite_local.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_rewrite.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/hostname.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_hostname.png)

### 五、QX 内正确配置应该如下图所示

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_right.png)

## 进入 iOS 自带的天气 app 自动获取当前定位(会有弹窗提醒)

### 确保自己手机内的天气 app 中只有一个城市的天气预报

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_weatherapp.png)

### 如果没有弹窗提醒请点击 [这里](https://t.me/hellcell321) 前往 Telegram 询问 @chiupam (此教程作者) or @PengYM (脚本作者)

## 六、进入 QX 配置 [task] 即添加任务请求

### 推荐 cron 时间 0 7-22/3 * * *

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/task_ui.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_1.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_2.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_3.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_4.png)

cron表达式：0 7-22/3 * * * (意思为 每天7-22点每3小时的第0分执行一次脚本，即7点、10点、13点，以此类推)

脚本远链：https://raw.githubusercontent.com/Peng-YM/QuanX/master/Tasks/caiyun.js 

图标远链：https://raw.githubusercontent.com/Orz-3/task/master/caiyun.png 来自[Orz-3 契阔大佬](https://github.com/Orz-3/task)

正确写法

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/caiyun_task_5.png)

