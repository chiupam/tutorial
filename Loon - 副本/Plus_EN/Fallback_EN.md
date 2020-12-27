# Fallback

The `Fallback` strategy group can be easily understood as Loon automatically test whether the nodes under the `Fallback` strategy group are available at intervals, and automatically select the first available node according to the node arrangement

## 1. Enter `Strategy Group` to add a strategy group

Please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group_EN.md) to jump to the `Manually add a policy group` tutorial, and return to setting `Fallback` after completing the operation Tutorials

## Two, set `strategy type`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `select`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `Fallback`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Fill in the alias of the strategy group according to the user’s personal preference, the unit of the `test interval` is `second`, the maximum timeout is The unit is `milliseconds`, modified according to the user's personal habits, it is recommended that `max timeout` be changed to `1000`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Test-URL` generally does not need to be modified

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_3.jpg)

## Three, add agent node

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The strategy group cannot perform delayed speed measurement, so only proxy nodes can be added

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) After following the first step, click `Add`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the filtered node from the list of `Filter subscription nodes`, it is strictly forbidden to select from the list of `Subscribe nodes`, otherwise There will be a Loon warning, or even a proxy server provider’s account, and other serious consequences

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Make sure there is a number in the `()` of `Filter` under `Subscription Filter` and click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Fallback_7.jpg)

# Say a few more words

- The newly added `Fallback` strategy group according to this tutorial has no substantive effect, and the `Fallback` strategy group needs to be nested as a sub-strategy group into the surrogate parent strategy group to play a substantive effect

- It must be noted that other sub-strategy groups cannot be nested under the `Fallback` strategy group, because the strategy group is not a node, and the strategy group does not delay testing.

- When adding a proxy node, it is strictly forbidden to select from the list of `subscribe nodes`, otherwise there will be a Loon warning, or even a proxy server provider’s ban.

- It is not allowed to have too many nodes in `Filtering Subscription Nodes`, it is recommended to be less than `5`, otherwise it is prone to Loon warnings and even proxy server provider bans and other serious consequences

- If you do not use regular expressions to filter suitable nodes, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex_EN.md) to learn regular expressions