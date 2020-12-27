# Regular filter subscription node

This tutorial needs to learn the basic writing of regular expressions. You can use regular expressions to filter the subscription nodes that users need. If you have not learned the regular expressions tutorial, please click [here]() to jump, and then do the following operations after learning

## One, subscribe node

If there is no subscription node, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy_EN.md) to jump to the `subscription node` tutorial

## Two, filter subscription nodes

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click the `Configuration` column below, and click `Filter subscription nodes`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the area as shown (+)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Fill in the name of the `filter subscription node` in the `alias` field, and name it according to the user's personal preference, but never The same name as the `subscription node` is allowed, otherwise a loop error will occur

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `included subscription`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the node subscribed in the step of `Subscribe to Node`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the upper right corner `Storage`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Filter Type`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) select `NameRegex`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_8.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click the `Required` field on the right side of `Regular expression` and enter the regular expression

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Check whether the node name appears below, if it does not appear, please double check whether the correct regular expression is entered, or `subscribe to the node `Is there a proxy node of this type in

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_10.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) After confirming that there are successfully filtered nodes, click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Remote_Filter_11.jpg)

# Say a few more words

- Fill in the name of the `filter subscription node` in the `alias` column, and name it according to the user's personal preference, but it is never allowed to be the same as the name of the `subscription node`, otherwise a loop error will occur

- This tutorial only allows users to filter subscription nodes. To allow the filter subscription nodes to function as an agent, the operation of `Russian doll` is required