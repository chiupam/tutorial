# PCC

The `PCC` strategy group can be easily understood as Loon automatically test the node delay under the `PCC` strategy group at intervals, and eliminate the node with the maximum delay set by the user, and lock the same node for the network access request of the same host name initiated by the user

## 1. Enter `Strategy Group` to add a strategy group

Please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md) to jump to the `Manually add a policy group` tutorial, and return to setting `PCC` after completing the operation Tutorials

## Two, set `strategy type`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `select`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `load-balance`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `random`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `pcc`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Generally, `Test-URL` does not need to be modified. The unit of `test interval` is `seconds`, and `max timeout` The unit is `milliseconds`, modified according to the user's personal habits, it is recommended that `max timeout` be changed to `1000`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_4.jpg)

## Three, add agent node

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The strategy group cannot perform delayed speed measurement, so only proxy nodes can be added

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) After following the first step, click `Add`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the filtered node from the list of `Filter subscription nodes`, it is strictly forbidden to select from the list of `Subscribe nodes`, otherwise There will be a Loon warning, or even a proxy server provider’s account, and other serious consequences

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Make sure there is a number in the `()` of `Filter` under `Subscription Filter` and click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/PCC_8.jpg)

# Say a few more words

-The newly added `PCC` strategy group according to this tutorial has no substantive effect. It is necessary to nest the `PCC` strategy group as a sub-strategy group into the surrogate parent strategy group to play a substantial role

-It must be noted that other sub-strategy groups cannot be nested under the `PCC` strategy group, because the strategy group is not a node, and the strategy group does not delay testing.

-When adding a proxy node, it is strictly forbidden to select from the list of `subscribe nodes`, otherwise there will be a Loon warning, or even a proxy server provider’s ban.

-It is not allowed to have too many nodes in `Screening Subscription Nodes`, it is recommended to be less than `10`, otherwise it is easy to appear Loon warnings, even proxy server provider bans and other serious consequences

-If you do not use regular expressions to filter suitable nodes, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md) to learn regular expressions

# Classic Case

-Regarding the situation that the policy type in the policy group is `PCC` and the available nodes under the policy group are `0`, it may be because the parent policy group did not select the `PCC` policy group as the proxy policy group

  -[Operation](https://t.me/Loon0x00/350123)