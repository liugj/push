# iOS两种推送形式的比较

## 证书推送
- 推送证书创建时便与固定的包名一一对应
如：
com.mysoft.mdev对应dev证书
com.mysoft.m对应prod证书
手机安装com.mysoft.mdev所获取到的设备token，只能通过dev证书进行推送，而无法通过prod证书推送

- 推送证书存在最长一年的有效期，到期后需更新（推送证书过期并不影响APP的使用，只影响推送功能)


## token推送
- token不区分包名，只要是同一个苹果开发者帐号下的应用，均可推送

- 只要苹果开发者帐号有效，则token长久有效

- 运行环境较证书推送要求高，使用时需根据实际情况评估