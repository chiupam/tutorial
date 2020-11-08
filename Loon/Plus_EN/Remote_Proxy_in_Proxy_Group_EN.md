# Nesting between nodes and policy groups

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Add the proxy node to the policy group to realize the proxy function, which is actually to make the policy form a `agent policy group `

## One, preliminary settings

-The user has not added a policy group as a nested node of `Proxy Policy Group`, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md) to jump `New child strategy group` tutorial to learn how to add a strategy group

-The user has successfully added a policy group as a nested node of `agent policy group`, please continue to browse the following tutorial

---

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click the `Configuration` column below, and click `Strategy Group`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Group.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click the policy group that needs to add the agent node, as shown in the figure below, the `manual selection` policy group as an example, click Manual selection`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Proxy_in_Proxy_Group_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click and set `Policy Type`, divided into 4 cases

-When the user wants to manually select a node, select the strategy type `select`, please go to `two` below this tutorial

-If the user wants the strategy group to play the following role, please click on the corresponding tutorial and browse the operations of the second and third steps in the jump tutorial

  -When the lowest latency node is automatically selected, that is, when the strategy type selects ʻurl-test`, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md) Jump to the `URL-Test policy group setting` tutorial, browse the operations of the second and third steps of the jump tutorial

  -When the available nodes are automatically selected, the strategy type is `fallback`, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md) to jump to `Fallback Setting the strategy group` tutorial, browse the second and third steps of the jump tutorial

  -When a node that meets the preset conditions automatically locks and agrees to a request for the same hostname, that is, when the policy type selects `load-balance`, please click [here](https://github.com/chiupam/tutorial/blob/master /Loon/Plus/PCC.md) Jump to the `PCC policy group setting` tutorial, browse the operations of the second and third steps of the jump tutorial

## Two. Only browse when the strategy type select `select`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Take the strategy type selection `select` as an example, click `Add`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Select_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the required `subscription node` or `filter subscription node from the list of `subscription nodes` or `filter subscription nodes` `, Click on the name

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Select_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Select_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Make sure there is a number in the `()` of `Filter` under `Subscription Filter` and click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Select_4.jpg)

# Say a few more words

-Only when the strategy type selects `select`, you can select from the list of `subscription nodes`, other policy types are strictly prohibited from being selected from the list of `subscription nodes`

-If users are interested in `Proxy Strategy Group`, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy.md) to jump to `Proxy Strategy Group` Tutorials