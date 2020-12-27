# MITM (Man in the Middle Attack)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Loon uses a man-in-the-middle attack to decrypt the https request. Decrypt the corresponding https request and response according to the configured hostname (domain name) and trusted CA certificate. After decryption, it can be split with Rule and URL Rewrite.

## General use of MITM

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In general use, if the MITM function is not enabled, the user may not be able to execute some scripts correctly, such as obtaining The script of Jingdong Cookie.

# Say a few more words

- Portal

 - [CA Certificate](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/CA_EN.md)

 - [hostname](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/hostname_EN.md)