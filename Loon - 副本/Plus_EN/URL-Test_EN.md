# URL-Test

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) ʻURL-Test` strategy group, by default it sends http requests to the configured url every 600s and chooses the fastest return data Node (Note: url-test does not support policy group as its sub-policy)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In layman’s terms, Loon automatically tests the delay of nodes in the ʻURL-Test` strategy group at intervals and automatically selects them for users Lowest latency node

- [TestFilght 2.14(215)](https://t.me/LoonNews/287) Update: Added tolerance parameter, used to compare the tolerance when switching nodes, the calculation method is as follows: the optimal node time in the previous speed measurement -Subtract the current speed measurement optimal node when the time is greater than tolerance, the node will be switched, the default is 100

  - In Loon's update instructions, the description of this part as "less than" is wrong, and correct should be "greater than"

## 1. Enter `Strategy Group` to add a strategy group

Please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group_EN.md) to jump to the `Manually add a policy group` tutorial, and return to the settings ʻURL- Test` tutorial

## Two, set `strategy type`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `select`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on ʻurl-test`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Fill in the alias of the strategy group according to the user's personal preference, the test interval unit is `second`, modify according to the user's personal habits, generally No need to modify

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The `tolerance` column is set according to the user's personal preference and the general delay of the proxy server provider. The calculation method has been introduced above, Self-understanding and self-setting

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Test-URL` generally does not need to be modified

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_4.jpg)

## Three, add agent node

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The strategy group cannot perform delayed speed measurement, so only proxy nodes can be added

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) After following the first step, click `Add`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the filtered node from the list of `Filter subscription nodes`, it is strictly forbidden to select from the list of `Subscribe nodes`, otherwise There will be a Loon warning, or even a proxy server provider’s account, and other serious consequences

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Make sure there is a number in the `()` of `Filter` under `Subscription Filter` and click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/URL-Test_8.jpg)

# Say a few more words

- The newly added ʻURL-Test` strategy group according to this tutorial has no substantive effect. It is necessary to nest the ʻURL-Test` strategy group as a sub-strategy group into the proxy parent strategy group to play a substantial role

- It must be noted that other sub-strategy groups cannot be nested under the URL-Test strategy group, because the strategy group is not a node, and the strategy group does not delay testing.

- When adding a proxy node, it is strictly forbidden to select from the list of `subscribe nodes`, otherwise there will be a Loon warning, or even a proxy server provider’s ban.

- It is not allowed to have too many nodes in `Screening Subscription Nodes`, it is recommended to be less than `10`, otherwise it is easy to appear Loon warnings, even proxy server provider bans and other serious consequences

- If you do not use regular expressions to filter suitable nodes, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex_EN.md) to learn regular expressions