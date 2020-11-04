## Loon Tutorial

- **The README_EN.md document is a simple translation of the README.md document. The operation of the hyperlink in this tutorial is still the Chinese illustration. The reader can set the iPhone language to Chinese and then operate.**

- Loon's Plus tutorial is stored in this folder.

- Please read the following **Disclaimer** carefully, any reader who clicks on the document in the tutorial will be deemed to have accepted this disclaimer.

### Disclaimer

- This tutorial is only for users who purchased the genuine Loon to learn how to use this software. I have never provided airport services or instigated mainland users to establish and use non-statutory channels for international networking without authorization.

- Through this tutorial, users use Loon to use illegal channels for international networking and conduct behaviors that violate the laws and regulations of mainland China and its regions. I am not responsible for the consequences of such users.

- This tutorial only teaches how to configure script functions, and will never provide any specific scripts that harm the legitimate interests of natural persons, legal persons, and unincorporated organizations, such as cracking scripts.

- Please do not use the script for any commercial or illegal purposes. I am not responsible for any consequences caused by such actions.

- Anyone who reads this tutorial in any way, directly or indirectly operates the steps in this tutorial, should read this statement carefully.

- I have the right to modify and supplement this disclaimer. Any reader who clicks on the document in the tutorial will be deemed to have accepted this disclaimer.

### Configuration column

The purpose is to improve the user's ability to customize the Loon configuration, and write tutorials in the order of the `configuration` column panel

#### Node

- [Single node](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Proxy.md) (add proxy node manually)

- [Subscription Node](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy.md) (subscribe to a collection of nodes, usually provided by the airport the user purchased)

- Screening subscription nodes (screening subscription nodes into proxy nodes that users need, reducing too many proxy nodes to appear in the policy group, and making it easy for users to choose the proxy nodes they need)

  - [Regular expression](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md) (Master the basic regular expression writing)

  - [Filter method with filter type `NodeSelect`](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter_NodeSelect.md) (manually filter nodes)
  
  - [Filtering method with the filter type `NameKeyword`](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter_NameKeyword.md) (Use keywords to filter subscription nodes, but nodes cannot be excluded)

  - [Filter method with filter type `NameRegex`](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter.md) (Use regular expression to filter subscription nodes)

-Use Sub-Store to filter subscription nodes (simple, efficient and convenient)

  - [Text Tutorial](https://www.notion.so/Sub-Store-6259586994d34c11a4ced5c406264b46)

  - [Video Tutorial](https://www.youtube.com/watch?v=VXlQ4kDgqSE&t=171s)

- [Nesting between node and policy group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy_in_Proxy_Group.md) (add proxy node under the policy group)

#### Strategy

- Loon without default proxy policy group

  - [Proxy Policy Group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy.md) (Understand the proxy policy group, with [understanding of global policy](https:// github.com/chiupam/tutorial/blob/master/Loon/Plus/Global_Group.md) tutorial)

  - [Understanding of the global strategy](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Global_Group.md) (the reason why the global agent must be used with the global strategy)
  
- [New Policy Group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md) (manually add a sub-policy group)

- Parent strategy group and child strategy group

  - [Correctly distinguish between parent policy group and child policy group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/TOP_Policy.md)

  - [Russian dolls-nesting between child and mother strategy groups](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Matryoshka.md)

- Three commonly used automatic strategy groups

  - [Set URL-Test Policy Group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md) (preferably the lowest latency)
  
  - [Set Fallback Policy Group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md) (health check)
  
  - [Set PCC policy group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/PCC.md) (the same host name locks the same node)
  
- Set SSID policy group

  - [Method 1: Setting of built-in ssid strategy group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/ssid.md) (This tutorial needs to understand more concepts and is relatively simple, Not flexible enough)
  
  - [Advanced Operation: Nesting of ssid Strategy Groups](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/ssid_Plus.md) (The operation is extremely cumbersome, but it is difficult to meet the requirements Understand, novices, users who are impatient, please detour) (unfinished)

  - [Method 2: Script method](https://t.me/cool_scripts/141) (SSID script is recommended, thanks to Peng-YM, please do not chat privately!)

#### Rules

- [What is a rule](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule_Summary.md) (the reason for the design rule in the agent software)

- [Single Rule](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule.md) (Add a local rule manually through the UI)

- [Subscription Rules](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Rule.md) (Subscribe to a collection of rules and select the parent policy group)

- [Recommendation Rules](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule_Recommend.md) (recommend common rules for novices)

- [Final Rules](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Final.md) (the rules of the rules)
 
#### Plugins

- [Preliminary understanding of plug-in functions](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Summary.md) (Powerful custom configuration artifact)

- [Add URL requirements and content format requirements in the plug-in](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Format.md) (a must-see for newbies)

- [Add a plugin](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin.md) (add a plugin)

- [Recommended plug-in URL](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Recommend.md) (organize more practical plug-ins for novices)

#### Copy

- [Rewrite](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rewrite.md)

#### Script

- [Learning basic cron expressions](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md) (modify the execution time of the timing script)

- Use scripts in Loon (from getting started to giving up)

  - [Getting Started-How to understand the necessary format of the three script statements](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format.md) (a must-see for novices)

  - [Elementary-How to understand a script configuration code](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_1.md) (Resolve the confusion of configuration scripts)

  - [Intermediate-How to write script configuration code into Loon to play a role](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_2.md) (required for script execution)
  
  - [Advanced-API Document Reference](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_3.md) (high-level players)
  
  - Abandon —— Script execution still fails (Sorry, I do not provide help in foreign languages.)

- [Add script file-download from URL](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) (download and store the script in ʻiCloud`)

- Local script (add script via UI method)

  - [Add local path script](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Local_JaveScript.md) (Select `Local` as the script location, need to match [Add script file-from URL Download](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md) tutorial study)
  
  - [Add remote link script](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_JaveScript.md) (Select `Remote` as the script location)
  
  - [Modify local script settings](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Modify.md) (Modify local script alias, cron expression, script location, etc. series of operations)

- Subscription script (lazy artifact)

  - [URL requirements and content format requirements in the subscription script](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Script_Format.md) (a must-see for newbies)

  - [Add subscription script](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Script.md) (the role of the subscription script function, the link requirements and content requirements of the subscription URL)

  - [Create a single local branch](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch.md) (Move the script in the subscription script to the local script, and you cannot modify the content of the local script. Only cron expressions can be modified)
  
  - [Create a single local branch and copy js](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch&Copy.md) (Move the script in the subscription script to the local script, you can modify the script Content, cron expression can also be modified)

#### DNS

- [DNS](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/DNS.md)

#### MITM

- [MITM](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/MITM.md) (Man in the middle attack)

- [Domain name](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/hostname.md) (two ways to add a domain name)

- [Certificate Management](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/CA.md) (causes and solutions about certificate pop-ups appear)

#### edit

- [Text Edit](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Configuration.md) (Loon’s configuration file)

- [Download from URL](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL_Download.md) (Download a complete set of configuration files from URL)

#### More

- [Network Sharing](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Network_Sharing.md) (Scientific Internet access can be achieved for devices under the same WiFi)

- [URL Schemes](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL_Schemes.md)

---

### Author statement

- For the convenience of readers, it is forbidden to forward this tutorial **link** or **content** to any social platform in the mainland. If found, chiupam will delete the library for processing

- In the course of writing tutorials, please go to the [Telegram Loon official group](https://t.me/Loon0x00) and @[chiupam](https://t.me/chiupam) if there are really highly demanded tutorials. Chiupam will Schedule time to speed up writing tutorials

- Non-professionals, if the user still cannot solve the user's problem after consulting the tutorial, they can go to [Telegram Loon Official Group](https://t.me/Loon0x00) and have a friendly exchange

- Energy is limited, compiling tutorials voluntarily, it is impossible to update the tutorials that users need in real time

- With limited intelligence, it is impossible to write such tutorials for problems that cannot be solved by oneself