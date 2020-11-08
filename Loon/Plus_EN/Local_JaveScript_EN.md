# Add local path script

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) This tutorial allows users to add a reference path in Loon as **local path** through the UI operation of Loon script

## Download script file from URL to icloud/Loon/Script

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/ Download_From_URL_EN.md) Jump to the `Add script file-download from URL` tutorial

## Fully understand the configuration code in the script file

**Take Jingtokyo bean sign-in script as an example**

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Read the configuration code in the script file, as shown in the code of `http-request` under `[Script]` in the figure below

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JD-DailyBonus_http-request.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Disassemble this configuration code according to the three script statement formats, ** clarify where you can modify and where you cannot. modify**

**If the user does not understand the three script statement formats, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format_EN.md) to jump to `Getting Started—— How to understand the necessary format of the three script statements `Tutorial**

-Items and locations that users cannot modify by themselves

  -`http-request` <===> script type

  -`https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean` <===> expression

-User can modify the items and fill in the location

  -`Get Jingdong cookie` <===> alias

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

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) select `Local`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `script name`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_8.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select the `JD_DailyBonus.js` file downloaded from the `Download from URL` function

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_9.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The correct wording is as shown in the figure below. After confirming that it is correct, click `Save` to complete the operation

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Local_Script_10.jpg)

# Say a few more words

-Loon is an open remote script link. If users do not need to modify the code in the script file, it is highly recommended to learn the `Add remote link script` tutorial and use the `Add remote link script` function, please click [here](https://github .com/chiupam/tutorial/blob/master/Loon/Plus/Remote_JaveScript.md) Jump to the `Add remote link script` tutorial

-Again, the premise of this tutorial is that the user needs to download the script to the icloud/Loon/Script folder through the `download from URL` function in advance and enable the `automatic synchronization` function in Loon. If the user has not done this step yet, Please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL_EN.md) to jump to the `Add script file-download from URL` tutorial