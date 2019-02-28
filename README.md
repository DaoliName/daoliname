# 道里名(DaoliName)

## 简介

道里名系统使用基于身份的公钥密码学技术，结合独创的"可压缩指纹(CF)"技术，允许使用任意Bit字符串做为公钥，如电子邮件地址，IP地址，手机号码等，有效的解决了一些基于传统PKI体系中复杂的身份认证，加密和密钥管理问题。

## 基本原理

对于所有可当做身份的Bit字符串，都需要向道里名注册。道里名提供身份注册服务，为所有基于身份的系统和软件提供在线查询服务。

**声明**

道里名系统中有如下三种角色：

* 身份注册系统

身份注册系统由道里名负责管理，为所有用户提供身份注册服务，允许注册任意字符串做为通信身份，道里名注册系统提供密钥生成以及身份查询服务。

* 发送端

发送端需要将自己的身份注册到道里名系统，并且在消息发送前，向道里名系统查询接收端身份的公钥信息，用来签名和加密数据。

* 接收端

接收端需要将自己的身份注册到道里名系统，并且在收到消息时，向道里名系统查询发送端身份的公钥信息，用来解密和验签数据。

**通信流程**

1. 数据发送端用户和接收端用户将各自的身份(邮箱地址，IP地址等)提前在道里名系统中注册，道里名注册系统生成私钥，由用户自己保存到安全系统(或者HSM)；
2. 通信开始前，由发送端向道里名系统发送请求，通过接收端身份查询接收端公钥信息；
3. 发送端通过自己的私钥对数据进行加密和签名，将消息发送出去；
4. 接收端收到发送端的消息后，也向道里名系统发送请求，获取发送端身份的公钥信息；
5. 接收端对消息进行解密并进行验签，如果验证通过则接收数据，否则丢弃；

## 应用场景

道里名将基于身份的密码技术应用在多种现有系统中，简化和替代现有解决方式。

* IPSec
* 邮件系统
* DNS安全
* 其它

## 技术理论

技术细节请参考[DaoliName.pdf](DaoliName.pdf)

## 计划安排

道里名v1版本计划将基于身份的密码技术应用在IPSec系统中，解决传统IPSec复杂的身份认证，加密和签名等问题。IPsec VPN已经在企业和个人中被广泛使用，道里名通过对开源IPsec VPN(libraswan)系统的改进，同时适配多种客户端， 加入基于身份的密码技术，以实现一整套IPSec解决文案。

1. IPSec VPN Server
2. IPSec for Windows
3. IPSec for Linux
4. IPSec for Mac
5. IPsec for Android
6. IPSec for IOS

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
