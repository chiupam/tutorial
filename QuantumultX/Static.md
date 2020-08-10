# 如何在Quantumult X中添加一个策略组

### 第一种方法：在UI界面添加(需要懂一点正则表达式)

第一步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/Static_1.1.png)

第二步：

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/Static_1.2.png)

完成~~~

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/QuantumultX/Static_1.3.png)

### 第二种方法：在编辑内添加(需要懂[policy]格式)

格式如下：

1、static=策略组名称, 节点1, 节点2, direct, proxy, reject, img-url=图标链接 

2、static=策略组名称, resource-tag-regex=正则筛选订阅, server-tag-regex=正则筛选节点, img-url=图标链接
