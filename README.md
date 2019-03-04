# 道里名(DaoliName)

## 简介

道里名系统使用"基于身份"的公钥密码学技术，结合独创的"可压缩指纹(CF)"技术，允许使用任意Bit字符串做为公钥，如电子邮件地址，IP地址，手机号码等，有效的解决了一些基于传统PKI体系中复杂的身份认证，加密和密钥管理问题。

## 基本原理

对于所有可当做身份的Bit字符串，都需要向道里名注册。道里名提供身份注册服务，为所有基于身份的系统和软件提供在线查询服务。

**声明**

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
6. IPSec for IOS
7. 小程序

## TODO

* Email System

## Useful Links

[DaoliName.pdf](https://tools.ietf.org/html/rfc5091)

[ID-based cryptography - wiki](https://en.wikipedia.org/wiki/ID-based_cryptography)

[IPSec -wiki](https://en.wikipedia.org/wiki/IPsec)

[S/MIME - rfc5751](https://tools.ietf.org/html/rfc5751)

[S/MIME - wiki](https://en.wikipedia.org/wiki/S/MIME)

[Security Architecture for the Internet Protocol - rfc4301](https://tools.ietf.org/html/rfc4301)

[DNS Security Introduction and Requirements - rfc4033](https://tools.ietf.org/html/rfc4033)
