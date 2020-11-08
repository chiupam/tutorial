# What is the rule

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) rule determines how to match by matching type when a request comes in, and how to choose the corresponding strategy

## Why proxy software needs to set rules

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Because when using proxy software, the user does not need to go through the proxy node to access the website inside the firewall, and when the user tries to access outside the firewall When you need to go through a proxy node to access

   - For example, users in Mainland China who directly connect to `www.baidu.com` will succeed, but will fail if they directly connect to `www.google.com`, but after setting the rules, using proxy nodes to access `www.google.com` will succeed

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In the `auto-distribution` mode, in order for Loon to use proxy nodes on demand, rules must be set for Loon

## Rule composition

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The rule is divided into three parts, namely: match type, match content, and strategy name

   - Such as: `DOMAIN-SUFFIX,twimg.com,PROXY`

## Match type

Match name|match type|description
-|-|-
Based on domain name suffix|DOMAIN-SUFFIX|None
Complete match based on domain name|DOMAIN|None
Based on domain name keywords|DOMAIN-KEYWORD|None
Matching based on the user agent string |USER-AGENT| according to the user-agent value of Http, supports wildcard matching with \*,?
Based on URL Regular|URL-REGEX|None
Based on the request IP range|IP-CIDR| is usually used for LAN matching
Based on IP as the country code|GEOIP|CN中国
Bottom matching|FINAL|If there is no matching rule, the default matching is used

## GeoiP

The IP-based location information comes from GeoLite2 Country. The GeoLiteZ database is an IP-based geographic location information database created by MaxMind. Available from www.maxmind.com.

## Examples demonstrate the role of understanding rules

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) The user in the following figure initiates an access request to `www.google.com`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/Ruld_Example.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In the `Strategy` column, `Proxy` represents the strategy and `[tunnel]香港01#GZCM` represents the proxy node

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) In the `rule` column, `DOMAIN-KEYWORD` represents the match type, `google` represents the match content, and `Proxy` represents Strategy name

It means that the user initiates an access request to `www.google.com`, and the matching type is `DOMAIN-KEYWORD` domain name keyword matching, the matching content is `google`, and the policy named `Proxy` is used. The lowest proxy node is `[tunnel]香港01#GZCM`

# Say a few more words

- Bottom matching, FINAL rule, please click [here](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Final_EN.md) to jump to the `Final rule` tutorial

# Reference

- [Loon Incomplete Tutorial-Rules-Rule](https://www.notion.so/2-967c1a07462c43ab88906162bec475a4)