# network sharing

Q: I have two devices. I downloaded Loon on one of them. Can the other device realize the scientific Internet access without downloading loon?

A: It can be achieved through the `Network Sharing` function.

## The role of network sharing

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon provides an HTTP/SOCKET5 proxy server to other devices under Wi-Fi, so that those under the same Wi-Fi Other devices, through the user manually set the HTTP proxy port and server in other devices to achieve scientific Internet access

## Necessary conditions for enabling this feature

-A device (the device that has downloaded Loon)

  -Personal hotspot must be turned off in the settings

  -The wireless LAN/Wi-Fi function must be turned on and connected to a Wi-Fi
  
  -The `Network Sharing` function must be turned on in Loon
  
-B device (the device that did not download Loon)

  -The wireless LAN/Wi-Fi function must be turned on and connected to the same Wi-Fi as the A device
  
  -Manually set the HTTP proxy configuration
  
## 1. Add the shortcut of `Network Sharing` to Loon's `Instrument` bar interface

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open the Loon interface and click on the designated area on the right of `Shortcut`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Long press the designated area on the right side of `Network Sharing` under the `Invisible` list, and drag it to the bottom of the `Visible` list

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Make sure that the `Visible` list appears `Network Sharing`, and then click `Return`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_2.jpg)

## 2. Operation steps on A device that has downloaded Loon

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click the card switch of `Network Sharing` on the Loon interface to enable the `Network Sharing` function

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Be sure to record the **gray ip address (ie server)** under the `Network Sharing` card, and here No `⛔️` emoticon pack appears

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click the `Network Sharing` card in the Loon interface

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Be sure to record the `HTTP proxy port`, and then please continue

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_A_6.jpg)

## Three, the operation steps of the B device without downloading Loon

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open the `Settings` in the B device, click Wireless LAN / Wi-Fi to enable the wireless LAN / Wi-Fi function

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Connect to the same wireless LAN / Wi-Fi as device A

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on the area as shown

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Find the `HTTP proxy` list and click on `Configure proxy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Select `Manual`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In the `Server` column, fill in the `gray ip address` under the `Network Sharing` card in the Loon of Device A

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In the `Port` field, fill in the `HTTP proxy port` in the `Network Sharing` card in the Loon of A device

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `storage` to realize the scientific Internet access of device B

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Network_Sharing_B_8.jpg)

## Special equipment-Windows 10

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Open the `Start` button of Windows 10

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Windows_1.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click the `Settings` button

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Windows_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Network and Internet`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Windows_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click on `Proxy`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Windows_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Fill in the ʻip address` in the `address` field under the list of `manually set proxy` and fill in the `port` field `HTTP proxy port`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Windows_5.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Click `Save`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Windows_6.png)

# Say a few more words

-Device A turns on the hotspot to device B, and then uses network sharing on device A to connect to device B scientifically. This will not work!

  -[Questions from enthusiastic netizens](https://t.me/Loon0x00/481366)

-MacBook users are asked to find out the tutorial for setting up the proxy for the notebook by themselves. This tutorial will not go into details

-The reason that the user is required to perform the first step is that there is no `Network Sharing` UI in the `Configuration` column of Loon. Currently, the `Network Sharing` function can only be enabled in the following two ways

  -`Network Sharing` card
  
  -Write relevant code in `text configuration` (this method is obsolete)

-For device A, after turning on the `Network Sharing` function, there will be a `⛔️` emoticon pack under the `Network Sharing` card, please turn on the wireless LAN / Wi-Fi function and connect to a Wi-Fi

-For device B, you cannot use this function to achieve scientific Internet access on some APPs. It may be that this type of APP uses `SOCKET5 proxy`. Please manually configure the SOCKET5 proxy server and port in the settings of this type of APP.