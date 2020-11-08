# The bottom line clause of the rule-`Final rule`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The subscription rules are only compiled by the community leaders, and cannot cover all the rules that require proxy nodes to access, there must be ` With the emergence of “Fish from the Net”, at this time, we need the bottom line clause of the rules—“Final Rule” to let users make the choice of “direct connection” or “proxy” access

## The reflection of `Final rule` in configuration

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click the `Configuration` column below, click `Example`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Example.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Found `[Rule]`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Example_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Find the last line of code under `[Rule]` `FINAL,Final`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Example_2.jpg)

## Understanding of `FINAL, Final`

`FIANL` is a necessary format requirement in Loon configuration, while `Fianl` is actually a strategy, and `Final` can be replaced with

-`DIRECT`

-~~REJECT~~ (It is indeed possible to write this, but it is tossing users, so it is not recommended)

-`Agent Strategy Group`

-`Mother Strategy Group`

## Understanding of the three situations of replacement

-`DIRECT`

  -That is, if the local rules and subscription rules are not matched, the direct connection strategy is used for the network request initiated by the user
  
  -For example: `FINAL,DIRECT` <===> directly select direct access
  
-`Agent Strategy Group`

  -That is, if the local rules and subscription rules are not matched, use the `proxy node` for the network request initiated by the user
  
  -For example: `FINAL, manual selection` <===> Manual selection >>> Proxy node (here, `manual selection` is just an example name, in fact, the proxy policy group name and node are set according to the user's needs)
  
-`Mother Strategy Group`

  -That is, if the local rules and subscription rules do not match, the network request initiated by the user requires the user to choose
  
  -For example: `FINAL,Final` <===> Final >>> DIRECT / Proxy (here `Fianl` is just an example name of the strategy group, in fact the name of the strategy group is set according to the user's needs)
  
## Deep understanding of the third situation

When the configuration says `FINAL,Final`, the following types of `parent policy groups` can be made through the nesting between the `child-parent policy groups`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Final.jpg)

As shown in the figure above, the user needs to manually preset the strategy to go when a fish slipping through the net appears. If the user chooses

-`DIRECT` built-in strategy group, namely directly select direct access

-`Proxy` parent policy group, the nesting situation is: Proxy >>> manually select >>> proxy node, that is, use proxy node to access

# Reference

-[Mind Map](https://t.me/Loon0x00/350927) from enthusiastic netizens, to understand the specific direction of the rules logically