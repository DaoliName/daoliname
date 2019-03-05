# DaoliName System (DaoliNS)

![DaoliName](images/logoh.png)

## Introduction to DaoliName System (DaoliNS)

DaoliName System (DaoliNS) is an “IBC” technology enabled Open Key Management System. Note the quote “IBC”, [this document](DaoliName.pdf) explains the reason.

Like usual IBCs, DaoliNS also needs a PKG (Private Key Generator) to publicize system public parameters: ( P, Q=[*s*]P ) where *s* is the so-called “Master secret key” of PKG.

There are several hundreds of root Certificate Authorities (CAs) certificates out there. For many years they have entered into all OSes, browsers and mobile apps. So DaoliNS at the top buys several certificates from popular root CAs, and have DaoliNS PKG system parameters (P, Q) certificate chain signed, so that they can be accepted by our clients, after download from the DaoliNS website in javascript.

CA issued certificates are quite commonly used by organizations, in particular by ones who make life out of webs, apps, and fancy services. These organizations are sufficiently resourceful for their CA issued certificates to reach their customers. It must be only because their customers who are ONLINE and pulling the OFFLINE certificates that can make the certificates fly even in lightspeed to the customers of the resourceful CA registrants.

DaoliNS buys certificates from root CAs to chain certify “IBC” root public parameters (P, Q) to enable DomainNS-like online availability of key management services to a mass volume of resource-less users.

Fortunately, unlike IBC (note, not quoted) inherently escrow user private keys, “IBC” enabled online key management service does not do key escrow in the infrastructure precisely the same as the PKI CAs do not do. The [slide deck](DaoliName.pdf) explains the technology like this: Let Alice play the role of PKG2. Collusion with PKG1 to fool herself is not an “do no evil” option for Alice.

Thus, let conventional crypto key management from the conventional PKI CAs continue serving resourceful organizations, to piggyback DaoliNS online crypto key management from “IBC” to commence a retail business serving a mass volume of resource-less, but online, dust users. We also hope that IPv6 addresses should route packets to the dusts too, as both are size compatible.

## 项目介绍

道里名系统使用"基于身份"的公钥密码学技术，结合独创的"可压缩指纹(CF)"技术，允许使用任意Bit字符串做为公钥，如电子邮件地址，IP地址，手机号码等，有效的解决了一些基于传统PKI体系中复杂的密钥管理问题。

道里名在线密钥管理系统提供身份注册服务，为所有基于身份的系统和应用软件提供在线查询服务，对于所有可当做身份的Bit字符串，都可以向道里名系统申请注册。

道里名系统中有如下角色：

* 身份注册系统

* 发送端签名

* 发送端加密

* 接收端解密

* 接收端验签

## 应用场景

道里名将基于身份的密码技术应用在多种现有系统中，简化和替代现有解决方式。

* IPSec
* 邮件系统
* DNS安全
* 其它

## 技术理论

技术细节请参考[DaoliName.pdf](DaoliName.pdf)

## 计划安排

道里名v1版本计划实现一套"基于身份"的注册系统，通过实现客户端程序，手机APP或者浏览器插件完成用户身份的注册。同时将基于身份的密码技术应用在IPSec系统中，解决传统IPSec复杂的身份认证，加密和签名等问题。IPsec VPN已经在企业和个人中被广泛使用，道里名通过对开源IPsec VPN(libraswan)系统的改进，同时适配多种客户端，加入基于身份的密码技术，以实现一整套IPSec解决文案。

1. IPSec VPN Server
2. IPSec for Windows
3. IPSec for Linux
4. IPSec for Mac
5. IPsec for Android
6. 小程序

## TODO

* Email System

## Useful Links

[DaoliName.pdf](DaoliName.pdf)

[ID-based cryptography - wiki](https://en.wikipedia.org/wiki/ID-based_cryptography)

[IPSec -wiki](https://en.wikipedia.org/wiki/IPsec)

[S/MIME - rfc5751](https://tools.ietf.org/html/rfc5751)

[S/MIME - wiki](https://en.wikipedia.org/wiki/S/MIME)

[Security Architecture for the Internet Protocol - rfc4301](https://tools.ietf.org/html/rfc4301)

[DNS Security Introduction and Requirements - rfc4033](https://tools.ietf.org/html/rfc4033)
