# 全局策略

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 当分流模式选择全局代理时，用户发起的访问请求全部使用代理节点，由于 Loon 没有默认代理策略组（类似于 Quantumult X 中的 `Proxy` 策略组），因而用户必须正确选择代理策略

## 一、在 `全局策略` 中选择代理策略

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 `Loon` 点击 `全局策略`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `Select` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `𝑷𝒓𝒐𝒙𝒚` （此名称不一定，原因请继续浏览下面的说明）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_7.jpg)

## 二、如何正确选择代理策略

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 每个策略追溯至最上层必定有一个分流在起作用，通过下面四张图片理解

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第一张图片：`国际媒体` 和 `国际网址` 需要代理节点才可以访问，这两条规则选择的母策略名为 `𝑷𝒓𝒐𝒙𝒚`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第二张图片：在策略组中看到母策略组 `𝑷𝒓𝒐𝒙𝒚` 选择的子策略组名为 `手动选择`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第三张图片：在子策略组 ` 手动选择` 下可以看到名为 `[隧道] 香港 01 #GZCM` 代理节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 第四张图片：当用户访问 `www.google.com` 时使用 `国际网站` 规则，该规则使用 `Proxy` 母策略组，该母策略组使用 `手动选择` 子策略组，该子策略组使用 `[隧道] 香港 01 #GZCM` 代理节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Global_Policy_4.jpg)

# 多说几句

- 关于 `母策略组` 和 `子策略组` 之间的关系，详细可以点击 [这里]() 跳转
