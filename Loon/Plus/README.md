## Loon 教程

- 此文件夹内存放 Loon 的 Plus 教程。

- 请仔细阅读以下**免责声明**，任何一经点击教程内文档的阅读者便视为您已接受此免责声明。

- **Foreign friends can read this [README.md](https://github.com/chiupam/tutorial/blob/master/Loon/Plus_EN/README.md) description, or access [the documents](https://github.com/chiupam/tutorial/tree/master/Loon/Plus_EN) in this folder.**

---

### Loon 官方

- [LoonManual](https://github.com/Loon0x00/LoonManual/blob/master/README.md)

- [Telegram：Loon0x00](https://t.me/Loon0x00)

- [Twitter：Loon0x00](https://twitter.com/loon0x00)

- [App Store 下载地址](https://itunes.apple.com/us/app/loon/id1373567447)

---

### 免责声明

- 此教程仅供正版购买 Loon 的用户学习如何使用此款软件，本人从未提供机场服务或教唆大陆用户擅自建立、使用非法定信道进行国际联网。

- 用户通过此教程利用 Loon 使用非法信道进行国际联网并实施违反中国大陆及其地区法律法规的行为，对此类用户造成的行为后果，本人概不负责。

- 此教程内只教授配置脚本功能的方法，绝对不会提供任何具体的损害自然人、法人、非法人组织的合法利益的脚本，例如破解脚本等。

- 请勿将脚本用于任何商业用途或者非法目的，对此类行为造成的任何后果，本人概不负责。

- 任何以任何方式阅读此教程的、直接或间接操作此教程内步骤的阅读者都应仔细阅读此声明。

- 本人有权更改、补充此免责声明的权利，任何一经点击教程内文档的阅读者便视为您已接受此免责声明。

---

### 配置栏篇

目的在于提高用户自定义 Loon 配置的能力，按 `配置` 栏面板顺序编写教程

[节点](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E8%8A%82%E7%82%B9)
[策略](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E7%AD%96%E7%95%A5)
[规则](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E8%A7%84%E5%88%99)
[插件](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E6%8F%92%E4%BB%B6)
[腹泻](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E5%A4%8D%E5%86%99)
[脚本](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E8%84%9A%E6%9C%AC)
[DNS](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#dns)
[Mitm](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#mitm)
[编辑](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E7%BC%96%E8%BE%91)
[更多](https://github.com/chiupam/tutorial/tree/master/Loon/Plus#%E6%9B%B4%E5%A4%9A)
[新功能](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/README.md#%E6%96%B0%E5%8A%9F%E8%83%BD)

#### 节点

- [单个节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Proxy.md)（手动添加代理节点）

- [订阅节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy.md)（订阅一个节点合集，通常是用户购买的机场提供）

- 筛选订阅节点（将订阅节点筛选成用户需要的代理节点，减少过多代理节点出现在策略组内，方便用户选择需要的代理节点）

  - [正则表达式](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md)（掌握基本的正则表达式写法）

  - [筛选类型为 `NodeSelect` 的筛选方法](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter_NodeSelect.md)（手动筛选节点）
  
  - [筛选类型为 `NameKeyword` 的筛选方法](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter_NameKeyword.md)（利用关键词筛选订阅节点，但不能排除节点）

  - [筛选类型为 `NameRegex` 的筛选方法](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter.md)（利用正则表达式筛选订阅节点）

- 利用 Sub-Store 筛选订阅节点（简单、高效、方便）

  - [图文教程](https://www.notion.so/Sub-Store-6259586994d34c11a4ced5c406264b46)（学习耗时较长，推荐先看视频教程再看图文教程）

  - [视频教程](https://www.youtube.com/watch?v=VXlQ4kDgqSE&t=171s)

- [节点与策略组之间的嵌套](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy_in_Proxy_Group.md)（将代理节点添加到策略组下）

#### 策略

- 没有默认代理策略组的 Loon 

  - [代理策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy.md)（理解代理策略组，搭配 [对全局策略的理解](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Global_Group.md) 教程）

  - [对全局策略的理解](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Global_Group.md)（全局代理必须需要搭配全局策略使用的原因）
  
- [新建策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md)（手动添加一个子策略组）

- 母策略组与子策略组

  - [正确分辨母策略组和子策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/TOP_Policy.md)

  - [俄罗斯套娃 —— 子母策略组之间的嵌套](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Matryoshka.md)

- 常用的三种自动策略组 

  - [设置 URL-Test 策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md)（优选最低延迟）
  
  - [设置 Fallback 策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md)（健康检测）
  
  - [设置 PCC 策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/PCC.md)（相同主机名锁定同一节点）
  
- 设置 SSID 策略组

  - [方法一：指定 ssid 下流量模式自动切换](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/ssid-trigger.md)（最简单快捷的方法，推荐新手使用）

  - [方法二：内置 ssid 策略组的设置](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/ssid.md)（此教程需要理解较多概念，而且较为单一，不够灵活）
  
  - [进阶操作：ssid 策略组的嵌套](https://github.com/ArriettyQAQ/loon_tutorial)（操作极其繁琐，但是满足需求，只是较难理解，新手、无耐心用户请绕道，鸣谢ArriettyQAQ大佬）

  - [方法三：脚本的方法](https://t.me/cool_scripts/141)（推荐使用 SSID 脚本，鸣谢Peng-YM大佬）

#### 规则

- [何为规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule_Summary.md)（代理软件中设计规则的原因）

- [单个规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule.md)（通过 UI 手动添加一个本地规则）

- [订阅规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Rule.md)（订阅一个规则合集并选择母策略组）

- [推荐规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule_Recommend.md)（为新手推荐较为常用规则）

- [Final规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Final.md)（规则的兜底条款）
 
#### 插件

- [初步了解插件功能](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Summary.md)（强大的自定义配置神器）

- [添加插件中对 URL 的要求及内容格式要求](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Format.md)（新手必看）

- [添加插件](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin.md)（添加一个插件）

- [推荐插件 URL](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Recommend.md)（为新手整理较实用性插件）

#### 复写

- [复写](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rewrite.md)

#### 脚本

- [基础 cron 表达式的学习](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md)（修改定时脚本的执行时间）

- 在 Loon 中使用脚本（从入门到放弃）

  - [入门 —— 如何看懂三种脚本语句的必备格式](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format.md)（新手必看）

  - [初级 —— 如何看懂一个脚本配置代码](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_1.md)（解开配置脚本的困惑）

  - [中级 —— 如何将脚本配置代码写入 Loon 内发挥作用](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_2.md)（执行脚本的必备操作）
  
  - [高级 —— API 文档参考](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_3.md)（高阶玩家）
  
  - [放弃 —— 仍然执行脚本失败](https://t.me/chiupam)（有偿代写脚本部分配置，收费标准：150元/次）

- [添加脚本文件 —— 从URL下载](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md)（将脚本下载并存储在 `iCloud`）

- 本地脚本（通过 UI 方法添加脚本）

  - [添加本地路径脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Local_JaveScript.md)（脚本位置选择 `Local` ，需要搭配 [添加脚本文件 —— 从URL下载](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) 教程学习）
  
  - [添加远程链接脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_JaveScript.md)（脚本位置选择 `Remote` ）
  
  - [修改本地脚本设置](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Modify.md)（修改本地脚本的别名、cron表达式、脚本位置等系列操作）

- 订阅脚本（懒人神器）

  - [订阅脚本中对 URL 的要求及内容格式要求](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Script_Format.md)（新手必看）

  - [添加订阅脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Script.md)（订阅脚本功能的作用，订阅的 URL 的链接要求和内容要求）

  - [创建单个本地分支](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch.md)（将订阅脚本内脚本移到本地脚本中，不可修改本地脚本内容，仅可修改 cron 表达式）
  
  - [创建单个本地分支并拷贝js](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch&Copy.md)（将订阅脚本内脚本移到本地脚本中，可修改脚本内容，也可修改 cron 表达式）

#### DNS

- [DNS](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/DNS.md)

#### MITM

- [MITM](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/MITM.md)（中间人攻击）

- [域名](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/hostname.md)（添加域名的两种方法）

- [证书管理](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/CA.md)（出现关于证书类弹窗的原因以及解决方法）

#### 编辑

- [文本编辑](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Configuration.md)（Loon 的配置文件）

- [从URL下载](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL_Download.md)（从 URL 下载一套完整的配置文件）

#### 更多

- [网络共享](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Network_Sharing.md)（可为处于同一 WiFi 下的设备实现科学上网）

- [URL Schemes](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL_Schemes.md)

---

### 新功能

- [内置代理策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Built-in_Proxy.md)（极度便利新手用户首次使用）

- [自定义策略组图标](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Custom_Icon.md)

---

### 友情链接

- [YouTuber Hell Cell 系列视频教程](https://www.youtube.com/channel/UCgjdfJbXYaFfC3Wxump37Mg)

- [YouTuber 北纬37度的大飛 系列视频教程](https://www.youtube.com/channel/UCXdlywuMV_a8jEZ4wV6669g)

---

### 作者声明

- 为了读者的方便，禁止将此教程 **链接** 或 **内容** 转发至大陆内任何社交平台上，如果发现，chiupam 将删库处理

- 教程编写中，确有高度需求的教程请前往 [Telegram Loon 官方群](https://t.me/Loon0x00) 并 @[chiupam](https://t.me/chiupam) 提出，chiupam 会安排时间加快写出教程

- 非专业人员，如果用户查阅教程后仍不能解决用户的问题，可以前往 [Telegram Loon 官方群](https://t.me/Loon0x00) 并进行友好交流

- 精力有限，义务编写教程，不可能即时更新用户需要的教程

- 智力水平有限，对于自身也无法解决的问题，不可能编写此类教程

