# sso
CAS认证服务，SSO（单点登录）

# 介绍

## CAS

CAS是一个单点登录框架， 是 Yale 大学发起的一个开源项目，旨在为 Web 应用系统提供一种可靠的单点登录方法，CAS 在 2004 年 12 月正式成为 JA-SIG 的一个项目。代码目前在[github](https://github.com/apereo/cas)上管理

## SSO

单点登录，英文全称：Single Sign On（SSO）

SSO是指在多个应用系统中，用户只需要登录一次就可以访问所有相互信任的应用系统。

**举例 **

这里我们就用淘宝和天猫举例来展示一下单点登录吧

![](https://upload-images.jianshu.io/upload_images/14481291-ef0cdb84d79e28d6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/14481291-dabdd3af30348638.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

如图，我们两个网站都是没有登录的，现在我们登录淘宝，然后不登录天猫直接刷新。

![](https://upload-images.jianshu.io/upload_images/14481291-e720af3a81129a7b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/14481291-10c9a30cc642489f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

由此，我们可以看出，在淘宝登陆上的时候，天猫自动登录了。这就是单点登录，一处登录，处处运行。

# 特征

CAS项目支持以下功能：

- CAS v1，v2和v3协议
- SAML v1和v2协议
- OAuth v2协议
- OpenID和OpenID连接协议
- WS-Federation被动请求者协议
- 通过JAAS，LDAP，RDBMS，X.509，Radius，SPNEGO，JWT，Remote，Trusted，BASIC，Apache Shiro，MongoDb，Pac4J等进行身份验证。
- 委派身份验证到WS-FED，Facebook，Twitter，SAML IdP，OpenID，OpenID Connect，CAS等。
- 通过ABAC授权，时间/日期，REST，Internet2的Grouper等。
- 通过Hazelcast，Ehcache，JPA，Memcached，Apache Ignite，MongoDb，Redis，DynamoDb，Couchbase等进行HA集群部署。
- 由JSON，LDAP，YAML，JPA，Couchbase，MongoDb，DynamoDb，Redis等支持的应用程序注册。
- 通过Duo Security，YubiKey，RSA，Google Authenticator等进行多因素身份验证。
- 用于管理日志记录，监视，统计，配置，客户端注册等的管理UI。
- 全局和每应用程序用户界面主题和品牌。
- 密码管理和密码策略实施。

CAS的基础建立在：[Spring Boot](https://projects.spring.io/spring-boot)和 [Spring Cloud](http://projects.spring.io/spring-cloud/)之上。

# 流程图

cas协议的流程图

![cas](https://upload-images.jianshu.io/upload_images/14481291-c6c66299c9b4c78f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

