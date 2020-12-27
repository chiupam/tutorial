# Correctly distinguish between parent policy group and child policy group

Correctly identifying the `mother strategy group` will help a lot to understand the logic of the `Russian doll`

## Method

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In fact, the `parent policy group` is very easy to identify, open Loon, click the `configuration` column below, and click `subscription rules`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/TOP_Policy_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) View the name of each subscription rule in blue font at the bottom left corner, except for the names of `DIRECT` and `REJECT`, The strategy group with the remaining name is `parent strategy group`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/TOP_Policy_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon, click on the `Configuration` column below, and click on the `Strategy Group`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Proxy_Group.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) View the parent strategy group named `𝐏𝐫𝐨𝐱𝐲`, you can see `𝐏𝐫𝐨𝐱𝐲` under the parent strategy group `Manual selection `, `preferred low latency`, `health detection` three sub-strategy groups

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/TOP_Policy_3.jpg)

# Say a few more words

- Except for `DIRECT` and `REJECT`, the reason is: Loon has built-in `DIRECT` and `REJECT` strategy groups, so it is impossible to have a strategy named `DIRECT` or `REJECT` in the `Strategy Group` panel group

- A strategy group named `DIRECT` or `REJECT` with a special font can appear, for example a strategy group named `𝐃𝐈𝐑𝐄𝐂𝐓`

- `Subscription rules` can only select a strategy group as a `parent strategy group`, not a `child strategy group`, but the `parent strategy group` is nested in other `parent strategy groups` to become a `child strategy group' `Outside the case