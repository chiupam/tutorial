# Elementary

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) I personally think that after setting the basic settings of Loon, every novice user hopes to add more in Loon Script, use the script to achieve the effect that the user wants, but do not know how to configure it. This tutorial will let novice users understand a script configuration instruction, and will describe how to add a script in the next tutorial

## Script

Currently, there are mainly the following script developers sorted out, in no particular order, here are four categories of script developers

- Script developers who write the configuration method of the script in the `script file`:

  - [lowking](https://github.com/lowking/Scripts/tree/master)
  
  - [lowking](https://github.com/lowking/Scripts/tree/master) (The developer announced that the warehouse is no longer maintained)
  
  - [toulanboy](https://github.com/toulanboy/scripts/tree/master)
  
  - [lxk0301](https://github.com/lxk0301/scripts) (JD series games)
  
  - [vinewx](https://ooxx.be/js)
  
  - [Peng-YM](https://github.com/Peng-YM/QuanX/tree/master/Tasks) (Caiyun Weather)
  
  - [NobyDa](https://github.com/NobyDa/Script/tree/master)
  
  - [evilbutcher](https://github.com/evilbutcher/Quantumult_X/tree/master)
  
- Script developers who write the configuration method of the script in `REAMDE.md`:

  - [chavyleung](https://github.com/chavyleung/scripts) 
  
  - [zZpiglet](https://github.com/zZPiglet/Task) (DiDi)
  
  - [chouchoui](https://github.com/chouchoui/QuanX)
  
  - [yichahucha](https://github.com/yichahucha/surge) (historical prices)
  
- Sometimes the script configuration method is written in the `script file`, and sometimes the script configuration method is written in the `REAMDE.md` script developer:

  - [chouchoui](https://github.com/chouchoui/QuanX)
  
  - [saza34](https://github.com/sazs34/TaskConfig) (all-in-one sign-in script)
  
- The developer of the script you together authors:

  - [nzw9314](https://github.com/nzw9314/QuantumultX/tree/master) (The author announced that it will officially stop updating on 2020.08.09, and the scripts that have been included before then can be used normally)
  
  - [songyangzz](https://github.com/songyangzz/QxScripts)
  
## How to make Loon execute these scripts

- For sign-in scripts that need to get the `cookie` class, for example: Jingtokyo bean sign-in script, you need

  - Add statements starting with `http-request` and `cron` under `[Script]` in the Loon configuration file, and add the domain name after `hostname = `under `[MITM]`
  
  - Follow the script configuration method to get the `cookie`
  
  - Occasionally need to be used with `BoxJs`
  
- For sign-in scripts that do not need to obtain the `cookie` class, for example: Jingdong mini game series script, you need

  - Add statements starting with `http-request` and `cron` under `[Script]` in the Loon configuration file, and add the domain name after `hostname = `under `[MITM]`
  
  - Occasionally need to be used with `BoxJs`
  
- For reminder only, for example: nCov-19 global epidemic notification script, you need

  - Add a statement starting with `cron` under `[Script]` in the Loon configuration file
  
- For some scripts with more complicated configuration methods, you need to write relevant codes in Loon's configuration file according to the configuration method description in the specific script

## A preliminary understanding of the instructions and configuration code in the script file

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Take the Beijing Tokyo Dou check-in script as an example. The script was developed by NobyDa (野比), because the script configuration instructions are written in the script file Inside, so first open [Script File](https://github.com/NobyDa/Script/tree/master/JD-DailyBonus)

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click Raw. This step is an important step. If the script configuration instructions are written in the script file, you need to click Raw to view

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Read the description at the beginning of the script file, look for related words such as `Loon configuration`, and clarify how to write in the configuration file in Loon Statement

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Look for words related to `instructions` to facilitate users to write script configuration code into Loon configuration and continue operation

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/JaveScript_1_4.jpg)

# Say a few more words

- If the user does not know what a script statement is, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format_EN.md) to jump to `Getting Started-How to understand The necessary format of three script statements` tutorial

- After reading this tutorial, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_2_EN.md) to jump to `Intermediate-How to write script configuration code Enter into Loon to play a role` tutorial, officially enter the relevant position in the Loon configuration file to write the relevant code of the script configuration

- For sign-in scripts, the user needs to add a `cron` statement under `[Script]`, or add it to the configuration through the UI, only if the user is **definite, affirmative, necessary, necessary**, this script will execute the sign-in task

# Thanks

- [NobyDa](https://github.com/NobyDa)