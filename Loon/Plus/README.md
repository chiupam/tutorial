# 进阶篇（目的在于提高用户自定义 Loon 配置的能力）

## 节点

- [正则表达式](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md)（掌握基本的正则表达式写法）

- [单个节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Proxy.md)（手动添加代理节点）

- [订阅节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy.md)（订阅一个节点合集，通常是用户购买的机场提供）

- [筛选订阅节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy.md)（利用正则表达式筛选订阅节点）

## 策略

- 母策略组与子策略组之间的逻辑关系

  - [正确分辨母策略组和子策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/TOP_Policy.md)

  - 理解 `俄罗斯套娃` 的小把戏 —— 子母策略组之间的嵌套

  - 添加子策略组（手动添加一个子策略组，注意此处是子策略组）

- 常用三种自动策略组的区别    

  - [URL-Test策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md)（优选最低延迟策略组）
  
  - [PCC策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/PCC.md)（相同主机名锁定同一节点策略组）
  
  - [Fallback策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md)（健康检测策略组）
  
  - SSID策略组（不写此教程是因为SSID策略组在 Loon 有逻辑问题，需要等待开发者修改逻辑关系）
  
## 规则

- 单个规则（手动添加一个规则）

- 订阅规则（订阅一个规则合集并选择母策略组）
 
## 复写

- 订阅复写（暂时不出此类教程，因为日常没有用到）

## 脚本

- [基础 cron 表达式的学习](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md)（修改定时脚本的执行时间）

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
