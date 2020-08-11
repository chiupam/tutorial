# 首次使用 Loon

## 一、通过 URL 下载功能下载一份简易版配置

先复制右侧这串地址：https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/Loon_example.conf

第一步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/peizhi.png)

第二步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL.png)

第三步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL_1.png)

第四步：

把上面复制的地址粘贴在下图的位置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL_2.png)

第五步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL_3.png)

## 二、配置证书

第一步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/zhengshuguanli.png)

第二步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_1.jpg)

第三步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_2.jpg)

第四步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_3.jpg)

第五步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_4.jpg)

第六步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_5.jpg)

第七步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_6.jpg)

第八步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_7.jpg)

第九步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_8.jpg)

## 三、添加订阅节点 (第三步与第四步必须连贯做)

第一步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy.png)

第二步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_2.png)

第三步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_3.jpg)

第四步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_4.jpg)

第六步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_5.jpg)

## 四、筛选订阅节点 (在此之前必须完成第三步)

第一步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter.png)

第二步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_1.jpg)

第三步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_2.jpg)

第四步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_3.jpg)

### 先学习正则表达式再往下看

- (A).*(B) or (A.*B|B.*A)
- 节点名既有A又有B 
- (A)|(B) or ^.*(A|B)
- 节点名有A或者B 
- ^((?!A).)*$
- 节点名不含有 A 
- (?!.*(A)).*(B) or ^(?!.*?A).*B
- 节点名不含有 A同时含有 B

### 看懂了再进行下一步

第五步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_4.jpg)

第六步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_5.jpg)

## 五、启动 Loon 连接

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/START.jpg)

## 六、选择策略以及子策略组的节点选择

第一步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group.jpg)

第二步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_1.png)

### 如果选择了 手动选择 策略组请进行下列操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_select.jpg)

### 如果选择了 优选地策略 or 健康检测 则不需要进行任何操作

## 完成~~~

# 逻辑图帮助理解

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Frist_end.png)

# 欢迎进入 Loon 官方 Telegram 频道 点击 [这里](https://t.me/Loon0x00) 跳转

