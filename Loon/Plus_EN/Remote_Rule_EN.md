# The necessity and advantages of the `subscription rule` function

`Subscription rules` allows users to avoid the need to manually add one rule after another in the local rules. The community has organized various rules for users to subscribe, saving users the trouble of adding rules locally.

## 1. Copy the raw link of the subscription rule

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) First find the rules that users need to subscribe to, and recommend using [Conners Hua](https://github.com/ConnersHua?tab =repositories), click [here](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset) to go to the github repository

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Take the example of subscribing to the rules of `China.list` (domestic rules), click on `China.list`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_Raw_China_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Raw`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_Raw_China_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `copy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_Raw_China_3.jpg)

## Second, confirm the selected strategy of `Subscription Rules`

There are three types of policy options for subscription rules, namely

- `DIRECT`

- `REJECT`

- `Agent Strategy Group`

- `Mother Strategy Group`

Because `China.list` is a Chinese rule, the strategy selection here is `DIRECT` (direct connection), and the strategy selection is `REJECT`, `agent strategy group`, and `parent strategy group. The similar operations are not explained here.


## Third, enter Loon subscription rules

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon, click on the `Configuration` tab below, and click `Subscription Rules`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_remote_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the area shown in the figure below (+)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_remote_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Paste the copied/copied address above to ʻURL` and fill in the branch alias

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_remote_China_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `DIRECT`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_remote_China_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) select `DIRECT`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_remote_China_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Rule_remote_China_6.jpg)

## Fourth, the order of subscription rules

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The order of the subscription rules is specified, and the order from top to bottom should be

- Go to the advertising category (strategy select `REJECT`)

- Domestic direct connection (strategy selection `DIRECT`)

- Foreign specific APP proxy (policy selection `agent strategy group` or `parent strategy group` {The name of this strategy may not be the same for each user, it depends on the name set by the user})

- Foreign agent class (strategy select `agent strategy group` or `parent strategy group` {The name of this strategy may not be the same for each user, it depends on the name set by the user})

# Say a few more words

- Ad rules recommend subscribing to NobyDa’s ad rules, please click [here](https://github.com/NobyDa/Script/tree/master/Surge) to jump

- Streaming media rules recommend subscribing to Conners Hua's rules, please click [here](https://github.com/ConnersHua/Profiles/tree/master/Surge/Ruleset) to jump to the github library

- Why is the name of `agent strategy group` or `parent strategy group" not necessarily the same for each user. It depends on the name set by the user. If you want to know the reason, please click [here](https://github.com/chiupam /tutorial/blob/master/Loon/Global_Policy.md) Jump and read `Three, proxy policy`

# Thanks

- [Conners Hua](https://github.com/ConnersHua?tab=repositories)

- [NobyDa](https://github.com/NobyDa)