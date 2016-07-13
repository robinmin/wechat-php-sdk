wechat-php-sdk
==============

本项目是在[dodgepudding/wechat-php-sdk](https://github.com/dodgepudding/wechat-php-sdk)
的基础上，对其中用了优问题的地方做了修正。主要修正点包括：

- 将项目中的私有成员变量与方法从private 修改为protected, 以便于字类对其中的bug进行重载覆盖；
- 文件[qywechat.class.php](https://github.com/robinmin/wechat-php-sdk/blob/master/qywechat.class.php)
中的函数`getUserId`实现错误予以修正--起始在修改了上一条的变量可访问性以后，本条已经可以在子类里面来重载了。

本项目的修改原则是尽量不动原来的代码，以便将来可替换。

