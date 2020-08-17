# 对 [general] 配置资源解析器等

## 一、复制下面一行代码

resource_parser_url=https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/resource-parser.js

server_check_url=http://www.gstatic.com/generate_204

geo_location_checker=http://ip-api.com/json/?lang=zh-CN, https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/IP_API.js

### 个人理解

- resource_parser_url 资源解析器

- server_check_ur 俗称的 ping 延迟 (如果没有此段代码在节点列表下拉不会显示节点延迟)

  - 等号后的地址还可以变更为：http://www.instagram.com/204 或者 http://www.google.com/generate_204 (不推荐这个地址)

- geo_location_checker 查看节点信息 (如果没有此段代码无法长按节点查看下级菜单)

## 二、进去 QX 进行配置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/dianji.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/bianji.png)

将上面的代码复制粘贴到下图所示位置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/general.png)

#### 注意：如果在上图中已经看到有 resource_parser_url=****** 这行代码，请直接覆盖而不是粘贴 (其他两个也同理)

### 正确配置如下图所示

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/general_right.png)

## 三、查看一下

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/resource_parser.png)

#### 如果没有看到如上图所示的界面请开关一次 VPN 连接

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/START-STOP.png)
![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/STOP-START.png)

# 鸣谢解析器作者

- Shawn [github库](https://github.com/KOP-XIAO)
