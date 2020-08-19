# 规则的兜底条款 —— `Final规则`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 订阅规则只是社区大佬整理而来的，并不能涵盖全部需要代理节点才能访问的规则，肯定有 `漏网之鱼` 的出现，这时候就需要规则的兜底条款 —— `Final规则` 来让用户做出 `直连` 或 `代理` 访问的选择

## `Final规则` 在配置中的体现

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `示例`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Example.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到 `[Rule]`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Example_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到 `[Rule]` 下最后一行代码 `FINAL,Final`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Example_2.jpg)

## 对 `FINAL,Final` 的理解

`FIANL` 是 Loon 配置中必备的格式要求，而 `Fianl` 实际上是一个策略，`Final` 处可以替换成

- `DIRECT`

- ~~~REJECT~~~ （确实可以这样写，但是折腾用户，因此不推荐）

- `代理策略组` 

- `母策略组`

## 对替换的三个情况的理解

- `DIRECT` 

  - 即如果本地规则和订阅规则都未匹配情况下，对用户发起的网络请求使用直连策略
  
  - 例如：`FINAL,DIRECT` === 直接选择直连访问
  
- `代理策略组` 

  - 即如果本地规则和订阅规则都未匹配情况下，对用户发起的网络请求使用 `代理节点`
  
  - 例如：`FINAL,手动选择` === 手动选择 >>> 代理节点 （代理策略组名称和节点按用户使用习惯设定）
  
- `母策略组`

  - 即如果本地规则和订阅规则都未匹配情况下，对用户发起的网络请求要求用户进行选择
  
  - 例如：`FINAL,Final` === Final >>> DIRECT / Proxy （母策略组名称和子策略组按用户使用习惯设定）
  
## 对第三种情况的深入理解

当配置中写着 `FINAL,Final` 时，通过 `子母策略组之间的嵌套` 可以做出以下类型的 `母策略组`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Final.jpg)

如上图所示，用户需要手动预设出现 `漏网之鱼` 时走的策略，如果用户选择

- `DIRECT` 内置策略组，即直接选择直连访问

- `Proxy` 母策略组，嵌套情况为：Proxy >>> 手动选择 >>> 代理节点，即使用代理节点访问

# 参考

- 来自热心网友的[思维导图](https://t.me/Loon0x00/350927)，从逻辑上理解规则的具体走向
