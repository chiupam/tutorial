# Add remote link script

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) This tutorial allows users to add a reference path in Loon as **remote path** through the UI operation of Loon script

## Fully understand the configuration code in the script file

**Take Jingtokyo bean sign-in script as an example**

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Read the configuration code in the script file, as shown in the code of `http-request` under `[Script]` in the figure below

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JD-DailyBonus_http-request.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Disassemble this configuration code according to the three script statement formats, ** clarify where you can modify and where you cannot. modify**

**If the user does not understand the three script statement formats, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format_EN.md) to jump to `Getting Started—— How to understand the necessary format of the three script statements `Tutorial**

- Items and locations that users cannot modify by themselves

  - `http-request` <===> script type

  - `https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean` <===> expression
  
  - `https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js` <===> Script remote link

- User can modify the items and fill in the location

  - `Get Jingdong cookie` <===> alias

## Add script via UI

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click the `Configuration` column below, and click `Add script`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the area as shown (+)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_1.jpg)

**Take adding http-request statement as an example**

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Script Type`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) select `http-request`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Write the script name in the `alias` column, name it according to the user's personal preference, preferably named after the script function

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Write the regular expression that matches the URL execution script in the `Expression` column, that is, `https:\/\/api \.m\.jd\.com\/client\.action.*functionId=signBean`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Script location`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) select `Remote`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_7_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Write the script remote link in the `Script link` column, namely `https://raw.githubusercontent.com/NobyDa/ Script/master/JD-DailyBonus/JD_DailyBonus.js`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_8_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The correct wording is as shown in the figure below. After confirming that it is correct, click `Save` to complete the operation

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_10_2.jpg)

# Say a few more words

- It is more recommended to use this method to add a single script, because the content of the script file in the remote link is modified, and the user can experience the new features brought by the script for the first time