<p align="center"><img src="https://www.discuz.net/static/image/common/logo.svg"></p>


## 关于 Discuz! Q

**[Discuz Q 官方](https://discuz.chat)**

## 安装方法

服务器环境需求为： **PHP 7.2.5+** 和 **MySQL 5.7+**, 并且需要安装 [Composer](https://getcomposer.org/)。

## 内测下载 Discuz! Q

首先注册[腾讯云帐号](https://cloud.tencent.com)并[实名认证](https://console.cloud.tencent.com/developer/auth)，然后在[API密钥管理](https://console.cloud.tencent.com/cam/capi)处新建一个密钥，运行列命令可下载 Discuz Q

```
composer config -g http-basic.cloud.discuz.chat ${QCLOUD_SECRET_ID} ${QCLOUD_SECRET_KEY}

composer create-project --prefer-dist qcloud/discuz --repository=https://cloud.discuz.chat
```

## 正式发布后下载 Discuz! Q

```
composer create-project --prefer-dist qcloud/discuz

cd resources/frame
npm install
npm run build
```


