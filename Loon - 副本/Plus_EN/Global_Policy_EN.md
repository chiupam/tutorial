# Global Strategy

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) When the global proxy is selected for the offloading mode, all access requests initiated by users use proxy nodes, because Loon does not have a default proxy policy group ( Similar to the `Proxy` strategy group in Quantumult X), the user must choose the proxy strategy correctly

## One, select the proxy strategy in the `global strategy`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open `Loon` and click `Global Strategy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Global_Policy_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Select`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Global_Policy_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `𝑷𝒓𝒐𝒙𝒚` (this name is not necessarily, please continue to browse the explanation below)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Global_Policy_7.jpg)

## Two, how to choose the proxy strategy correctly

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Every strategy traced back to the top level must have a diversion in action, understand through the following four pictures

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The first picture: `International Media` and `International Websites` need proxy nodes to be able to access, these two rules are selected The parent strategy is called `𝑷𝒓𝒐𝒙𝒚`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Global_Policy_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The second picture: See the parent strategy group `𝑷𝒓𝒐𝒙𝒚` in the strategy group. The selected child strategy group is named `Manual Choose`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Global_Policy_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The third picture: Under the sub-strategy group `Manual selection`, you can see the name `[tunnel]香港01 # GZCM` proxy node

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Global_Policy_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Fourth picture: When a user visits `www.google.com`, use the `International Website` rule, which is used `Proxy` parent policy group, the parent policy group uses the `manual selection` child policy group, and the child policy group uses `[tunnel] Hong Kong 01 #GZCM` Proxy node

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Global_Policy_4.jpg)

# Say a few more words

- For the relationship between `parent strategy group` and `child strategy group`, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/TOP_Policy_EN.md) to jump to details