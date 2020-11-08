# Certificate issues

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) If there is any reminder about **certificate** related words in the pop-up window when running Loon, please follow the steps an examination

## How to check whether the certificate is consistent

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open Loon and click the `Configuration` column below, and click `Certificate Management`

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Record the number displayed in the area as shown in the figure below and record it as `Certificate No. 1`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open the phone **Settings** >>> **General** >>> **About this machine**> >> **Certificate Trust Settings** (Not taking screenshots in this step is because of lazy cancer. You can follow this step to find the entrance on ios 13 and above)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Record the number displayed in the area as shown in the figure below and record it as `Certificate No. 2`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Contrast whether `Certificate No. 1` and `Certificate No. 2` are the same

-When they are the same, but "installed but not trusted by the system" is displayed below, please continue with the following tutorial operations **Trust Certificate**

-If it is inconsistent, please continue to follow the tutorial below **Reinstall the certificate**

## Trust Certificate

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open the phone **Settings** >>> **General** >>> **About this machine**> >> **Certificate Trust Settings** (Not taking screenshots in this step is because of lazy cancer. You can follow this step to find the entrance on ios 13 and above)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Find the certificate with the same number as the user’s `Certificate No. 1`, click the button on the right to make the `gray button` become ` Green button `to complete the **trust certificate** operation

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_8.jpg)

## Reinstall the certificate

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open the phone **Settings** >>> **General** >>> **Description File** >> > **Number of LOON CA No. 2 Certificate** (This step does not take a screenshot because of lazy cancer. You can follow this step to find the entrance on the ios 13 system)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Remove description file` and enter the password

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Remove`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Then open Loon and click the `Configuration` column below, and click `Certificate Management`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Certificate_UI.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Generate new CA certificate`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Install CA Certificate`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In the page that jumps out, click `Allow`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open the phone settings and click `Downloaded description file`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) After clicking on `install`, the verification steps appear, please enter the password to verify

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Go back to the phone settings and click `General`, then click `About this machine`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Certificate Trust Settings`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click the button to turn the `gray button` into a `green button` to complete the operation

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/mitm_8.jpg)

# Say a few more words

-The number after the certificate is very important, users need to check it accurately, and whether there is a word "installed but not trusted by the system". To determine if the user needs to **reinstall the certificate** or **trust the certificate**

-The time of making the tutorial is 1 am, so the certificate numbers in most screenshots in the tutorial are not strictly the same. The user needs to determine whether to perform the operation of **reinstalling the certificate** or **trusting the certificate** according to the actual situation.