# 全局代理与全局策略

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Q：为什么选择全局代理后的访问请求依然不能使用代理节点？

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) A：可能是因为用户没有正确选择全局策略。

## 全局直连、自动分流、全局代理（小白语句）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 全局直连：顾名思义，用户发起的访问请求全部使用国内网络

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 自动分流：依据用户设置的规则，对用户发起的访问请求按规则选择代理或直连

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 全局代理：顾名思义，用户发起的访问请求全部使用代理，即科学上网

## 全局策略

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 当分流模式选择全局代理时，全局策略必须正确选择代理策略，原因是 `Loon` 没有默认代理策略组

## 代理策略

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 每个策略追溯至最上层必定有一个分流在起作用，通过下面四张图片理解

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第一张图片：`国际媒体` 和 `国际网址` 需要代理节点才可以访问，这两条规则选择的母策略名为 `Proxy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第二张图片：在策略组中看到母策略组 `Proxy` 选择的子策略组名为 `手动选择`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第三张图片：在子策略组 ` 手动选择` 下可以看到名为 `[隧道] 香港 01 #GZCM` 代理节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第四张图片：当用户访问 `www.google.com` 时使用 `国际网站` 规则，该规则使用 `Proxy` 母策略组，该母策略组使用 `手动选择` 子策略组，该子策略组使用 `[隧道] 香港 01 #GZCM` 代理节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_4.jpg)
