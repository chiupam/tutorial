# 规则的兜底条款 —— `Final规则`

订阅规则只是社区大佬整理而来的，并不能涵盖全部需要代理节点才能访问的规则，肯定有 `漏网之鱼` 的出现，这时候就需要规则的兜底条款 —— `Final规则` 来让用户做出 `直连` 或 `代理` 访问的选择

## `Final规则` 在配置中的体现

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `示例`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Example.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到 `[Rule]`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Example_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 找到 `[Rule]` 下最后一行代码 `FINAL,Final`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Example_2.jpg)

## 对 `FINAL,Final` 的理解

`FIANL` 是 Loon 配置中必备的格式要求，而 `Fianl` 实际上是一个策略，`Final` 处可以替换成

- `DIRECT`

- `代理策略组` 

- `母策略组`
