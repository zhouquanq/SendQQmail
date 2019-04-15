# SendQQmail

## 简述

**SendQQmail**是利用 [PHPMailer](https://github.com/PHPMailer/PHPMailer) 类给QQ发送邮件的

要求：

* PHP 打开 sockets 扩展
* PHP 打开 openssl 的支持 （都可以通过phpinfo()查看是否开启）

## 目录说明

```
SendQQmail					根目录
├─src						应用目录
│  ├─PHPMailer 				PHP邮件发送类
│  ├─PHPMailer.class.php 	二次封装 方便使用
│  ├─index 					入口文件
```

## 使用

### 1.克隆代码

```
git clone https://github.com/zhouquanq/SendQQmail.git

```

### 2. QQ邮箱开启SMTP 协议

所有的主流邮箱都支持 SMTP 协议，但并非所有邮箱都默认开启，您可以在邮箱的设置里面手动开启。
第三方服务在提供了账号和密码之后就可以登录 SMTP 服务器，通过它来控制邮件的中转方式。


### 3.获取授权码

SMTP 服务器认证密码，需要妥善保管（PS：密码直接没有空格）。

