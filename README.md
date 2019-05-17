# DaoliName System (DaoliNS)

![DaoliName](images/logoh.png)

## Introduction to DaoliName System (DaoliNS)

DaoliName System (DaoliNS) is an “IBC” technology enabled Open Key Management System. Note the quote “IBC”, [this document](DaoliName.pdf) explains the reason.

There are several hundreds of root Certificate Authorities (CAs) certificates out there. For many years they have entered into all OSes, browsers and mobile apps. So DaoliNS at the top buys several certificates from popular root CAs, and have DaoliNS PKG system parameters (P, Q) certificate chain signed, so that they can be accepted by our clients, after download from the DaoliNS website in javascript.

CA issued certificates are quite commonly used by organizations, in particular by ones who make life out of webs, apps, and fancy services. These organizations are sufficiently resourceful for their CA issued certificates to reach their customers. It must be only because their customers who are ONLINE and pulling the OFFLINE certificates that can make the certificates fly even in lightspeed to the customers of the resourceful CA registrants.

Fortunately, unlike IBC (note, not quoted) inherently escrow user private keys, “IBC” enabled online key management service does not do key escrow in the infrastructure precisely the same as the PKI CAs do not do. The [slide deck](DaoliName.pdf) explains the technology like this: Let Alice play the role of PKG2. Collusion with PKG1 to fool herself is not an “do no evil” option for Alice.

Thus, let conventional crypto key management from the conventional PKI CAs continue serving resourceful organizations, to piggyback DaoliNS online crypto key management from “IBC” to commence a retail business serving a mass volume of resource-less, but online, dust users. We also hope that IPv6 addresses should route packets to the dusts too, as both are size compatible.

## 项目介绍

道里名系统使用"基于身份"的公钥密码学技术，结合独创的"可压缩指纹(CF)"技术，允许使用任意Bit字符串做为公钥，如电子邮件地址，IP地址，手机号码等，有效的解决了一些基于传统PKI体系中复杂的密钥管理问题。

道里名在线密钥管理系统提供身份注册服务，为所有基于身份的系统和应用软件提供在线公钥查询服务，对于所有可当做身份的Bit字符串，都可以向道里名系统申请注册。

道里名APP有如下功能：

* 身份注册(目前仅支持邮件，后续加入手机号,社交帐号等多种身份)

* 文件加密分享(无需注册)

* 文件签名分享

* 在线解密

* 在线验签(无需注册)

* 云端存储

## TODO

* 查找和添加朋友

* 用户身份管理

* 群加密

* 语音识别加密

## 技术文档

1. [IBC_IoT.pdf](IBC_IoT.pdf)

2. [IBC_IoT_eng.pdf](IBC_IoT_eng.pdf)

3. [DaoliName.pdf](DaoliName.pdf)

## Useful Links

[IBC_IoT.pdf](IBC_IoT.pdf)

[IBC_IoT_eng.pdf](IBC_IoT_eng.pdf)

[DaoliName.pdf](DaoliName.pdf)
