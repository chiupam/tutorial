# Built-in ssid strategy group

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Some users use routers to support walls, hoping that Loon's proxy distribution can be automatically switched to the direct connection state, and users do not need to enter manually Open the global direct connection mode in Loon, then you can use Loon's built-in ssid strategy group

## Note

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon's built-in ssid strategy group nesting is difficult to understand. This tutorial requires users to understand the role of rules and proxy strategies Group concept, tutorial link is provided below

-[What is a rule](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule_Summary_EN.md)

-[Proxy Policy Group](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy_EN.md)

## Steps

The operation steps are divided into two steps. The first step is to create a new ssid policy group, and the second step is to change the policy group selection of subscription rules

### New ssid policy group

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click on the `Configuration` column below

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `Strategy Group`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click the upper right corner +

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Enter the name of the strategy group in the alias field, and it is recommended to enter the SSID

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Strategy Type`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) select `ssid`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `default`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) It is recommended to choose the proxy strategy group. For the reasons, please see the analysis below in this tutorial

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_8.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `Cellular Data`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) It is recommended to choose an agent strategy group

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_10.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Add`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_11.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Enter the name of the router that the user has supported

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_12.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Then click `OK`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_13.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) select `DIRECT`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_14.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the upper right corner `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_1_15.jpg)

### Change the policy group selection of subscription rules

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon, click on the `Configuration` column below

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Subscription Rules`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the branch that requires proxy, such as the `Global` branch in the figure. For the reason, please see the analysis below this tutorial

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Slide the rule to the left

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Edit`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `Strategy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the ssid strategy group you just created, that is, the strategy group named SSID

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Save` in the upper right corner

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/ssid_2_8.jpg)

## Say a few more words

-Analyze:

  -The proxy policy group is selected in `default` because when the user connects to a WiFi that is not set to and does not have a router to support the wall, Loon still needs to use the split mode, otherwise the user cannot proxy
  
  -The `Global` subscription rule is a rule that requires an agent to be able to access successfully, so every subscription rule that needs to use an agent node needs to perform the second step, otherwise it may not have the effect that the user wants
  
  -In the lazy configuration text, the name of the proxy policy group will generally be named Proxy
  
  -If the user uses customized configuration text, please select the proxy policy group according to your own situation

-If the user wants to set up some APP, such as YouTube, when using the router to support the wall, the method is similar, except that the rule selected in the second step is the YouTube subscription rule

-If the policy group under the subscription rule is DIRECT (direct connection) or REJECT (reject), do not proceed to the second step. The reason is: For example, when users in mainland China use WeChat, they will never use proxy nodes, right?