# Loon 保姆教程

# 法律声明

- 此教程仅供正版购买 Loon 的用户学习如何使用 Loon 这款软件，作者从未也绝不会提供机场服务或教唆大陆用户科学上网

- 为了读者的方便，禁止将此教程 `链接` 或 `内容` 转发至大陆内任何社交平台上，如果发现，作者将删库处理

## 基础篇

目的在于用户基本能利用 Loon 实现代理功能

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

## 进阶篇

目的在于提高用户自定义 Loon 配置的能力，按 `配置` 栏面板顺序编写教程

### 节点

- [正则表达式](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md)（掌握基本的正则表达式写法）

- [单个节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Proxy.md)（手动添加代理节点）

- [订阅节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy.md)（订阅一个节点合集，通常是用户购买的机场提供）

- [筛选订阅节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter.md)（利用正则表达式筛选订阅节点）

- [节点与策略组之间的嵌套](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy_in_Proxy_Group.md)（将代理节点添加到策略组下，实现代理功能）

### 策略

- 没有默认 `Proxy` 代理策略组的 Loon 

- 母策略组与子策略组之间的逻辑关系

  - [正确分辨母策略组和子策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/TOP_Policy.md)

  - 理解 `俄罗斯套娃` 的小把戏 —— [子母策略组之间的嵌套](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Matryoshka.md)（未写）

  - [新建子策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md)（未写）（手动添加一个子策略组，注意此处是子策略组）

- 常用三种自动策略组的区别    

  - [URL-Test策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md)（优选最低延迟）
  
  - [Fallback策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md)（健康检测）
  
   - [PCC策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/PCC.md)（相同主机名锁定同一节点）
  
  - SSID策略组（不写此教程是因为SSID策略组在 Loon 有逻辑问题，需要等待开发者修改逻辑关系）
  
### 规则

- [单个规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule.md)（未写）（手动添加一个规则）

- [订阅规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Rule.md)（未写）（订阅一个规则合集并选择母策略组）
 
### 复写

- 订阅复写（暂时不出此类教程，因为日常没有用到）

### 脚本

- [基础 cron 表达式的学习](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md)（修改定时脚本的执行时间）

- 本机JS文件

  - [添加脚本文件 - 从URL下载](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md)（未写）（利用 `从URL下载脚本` 功能并将脚本存储在 `iCloud` 中）

- 本地脚本（通过 UI 方法添加脚本）

  - [添加本地路径脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Local_JaveScript.md)（未写）（脚本位置选择 `Local` 的方法，需要搭配 `本机JS文件` 的 `添加脚本文件` 教程学习）
  
  - [添加远程链接脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_JaveScript.md)（未写）（脚本位置选择 `Remote` 的方法）

- 订阅脚本

  - [添加订阅脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Script.md)（未写）（懒人必备，或者动手能力强的用户可高度自定义脚本合集{需要搭配 `github` 使用}）

  - [创建单个本地分支](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch.md)（未写）（将订阅脚本内需要的脚本移到本地脚本中，不可修改本地脚本内容，可修改 cron 表达式）
  
  - [创建单个本地分支并拷贝js](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch&Copy.md)（未写）（将订阅脚本内需要的脚本移到本地脚本中，可修改脚本内容，仅可修改 cron 表达式）

### DNS

- DNS服务器（本人不知道 `DNS服务器` 有什么作用，而且日常中很少接触此类问题，因此略过关于 `DNS服务器` 的教程）

### 插件

- [添加插件](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin.md)（未写）（一个强大的功能，特别对于频繁使用 `Tiktok` 的用户）

### MITM

- [域名](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/hostname.md)（未写）（hostname）与添加域名（hostname）的两种方法

- [证书管理](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/p12.md)（未写）（出现关于证书类弹窗的原因以及解决方法）

# 作者声明

- 教程编写中，确有高度需求的教程请前往 [Telegram Loon 官方群](https://t.me/Loon0x00)并 @chiupam 提出，作者会安排时间加快写出教程

- 作者非开发人员，不可能通过此教程完全解决用户所有问题，如果用户查阅教程后仍不能解决用户的问题，可以前往 [Telegram Loon 官方群](https://t.me/Loon0x00)并进行友好交流

- 作者精力有限，义务编写教程，不可能即时更新用户需要的教程

- 作者智力水平有限，对于自身也无法解决的问题，不可能编写此类教程

