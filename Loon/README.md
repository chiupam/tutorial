# Loon 保姆教程

## 基础篇（目的在于用户基本能利用 Loon 实现科学上网）

- [首次使用 Loon 教程](https://github.com/chiupam/tutorial/blob/master/Loon/Frist.md) （如导入其他懒人配置的用户请自行根据懒人配置顶部说明进行操作，选择性阅读此教程的步骤）

- [首次使用 BoxJs 配置](https://github.com/chiupam/tutorial/blob/master/Loon/BoxJS.md) （已有官方教程，请点击 [这里](https://chavyleung.gitbook.io/boxjs/) 跳转）

- [签到类脚本的本地配置方法——以京东京豆签到脚本为例](https://github.com/chiupam/tutorial/blob/master/Loon/JD_DailyBonus_1.md) （通过学习配置京东京豆签到脚本，学会如何自行添加脚本）

- [脚本的高级配置方法](https://github.com/chiupam/tutorial/blob/master/Loon/JD_DailyBonus_1.md) （不要投机取巧，高级配置方法的链接在本地配置方法文档内）

- [彩云天气脚本配置方法](https://github.com/chiupam/tutorial/tree/master/caiyun) （学会京东京豆签到脚本配置再整一个彩云天气脚本配置加强学习）

- [脚本执行时间](https://github.com/chiupam/tutorial/blob/master/Loon/cron.md) （学习完基本可以学会 cron 的写法）

- [全局代理与全局策略](https://github.com/chiupam/tutorial/blob/master/Loon/Global_Policy.md) （解决使用全局代理时不走节点流量的问题）

- [订阅规则](https://github.com/chiupam/tutorial/blob/master/Loon/Rule.md) （仅限策略选择为 `DIRECT`、`REJECT`、`PROXY`{此名称不一定}时学习）

- [订阅 Netflix 规则](https://github.com/chiupam/tutorial/blob/master/Loon/Rule_Netflix.md) （订阅特殊类 app 规则并选择特殊代理节点）

- [新创策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Proxy_Group.md) （搭配上面 `订阅 Netflix 规则` 学习效果更佳）

- [Final策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Final.md) （图解 `Fianl` 策略组的作用）

## 进阶篇（目的在于提高用户自定义 Loon 配置的能力）

### 节点

- 手动添加代理节点

- 订阅节点

- 筛选订阅节点（利用正则表达式筛选订阅节点）

### 策略

- 正确分辨母策略组和子策略组并理解 `俄罗斯套娃` 的小把戏

- 添加策略组（手动添加一个子策略组，注意此处是子策略组）

- 常用三种自动策略组的区别    

  - [URL-Test策略组](https://github.com/chiupam/tutorial/blob/master/Loon/URL-Test.md)     
  
  - [PCC策略组](https://github.com/chiupam/tutorial/blob/master/Loon/PCC.md)     
  
  - [Fallback策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Fallback.md)
  
  - SSID策略组（不写此教程是因为SSID策略组在 Loon 有逻辑问题，需要等待开发者修改逻辑关系）
  
## 规则

- 手动添加单个规则

- 订阅规则（订阅一个规则合集并选择母策略组）
 
## 复写

- 订阅复写（暂时不出此类教程，因为日常没有用到）

## 脚本

- 本机JS文件（需要搭配 `添加本地脚本` 的 `添加本地路径脚本` 教程学习）

  - 添加脚本文件（利用 `从URL下载脚本` 功能并将脚本存储在 `iCloud` 中）

- 本地脚本

  - 添加本地路径脚本（脚本位置选择 `Local` 的方法）
  
  - 添加远程链接脚本（脚本位置选择 `Remote` 的方法）

- 订阅脚本

  - 添加订阅脚本（懒人必备，或者动手能力强的用户可高度自定义脚本合集{需要搭配 `github` 使用}）

  - 创建单个本地分支（将订阅脚本内需要的脚本移到本地脚本中，可修改本地脚本内容，可修改 cron 表达式）
  
  - 创建单个本地分支并拷贝js（将订阅脚本内需要的脚本移到本地脚本中，不可修改脚本内容，仅可修改 cron 表达式）

## DNS

- DNS服务器（本人不知道 `DNS服务器` 有什么作用，而且日常中很少接触此类问题，因此略过关于 `DNS服务器` 的教程）

## 插件

- 添加插件（一个强大的功能，特别对于频繁使用 `Tiktok` 的用户）

## MITM

- 域名（hostname）与添加域名（hostname）的两种方法

- 证书管理（出现关于证书类弹窗的原因以及解决方法）

# 教程编写中，确有高度需求的教程请前往 [Telegram Loon 官方群](https://t.me/Loon0x00)并 @chiupam 提出
