# 搭建后端
如果没有特别注明，以下步骤皆为参考[微信小程序之PHP服务器搭建](https://blog.csdn.net/longjialin93528/article/details/79727237) 
- 在阿里云购买了的 ECS 主机，使用了云集的 LAMP(PHP 7.0) 镜像。华东区最便宜的主机大概 25RMB 一个月，流量 0.08RMB/GB，或者 20RMB/1M/月。
- 用 SSH 密钥使用 putty 远程连接。
- 申请域名和备案（optional）。这里面有一个坑，微信小程序要求后台必须 HTTPS, HTTPS 意味着需要证书，证书阿里云是可以有免费申请，但是好像不能绑在 IP 上，而且 IP 这种不稳定的东西我也不想用来绑证书。所以还是绑域名，可是绑域名到国内主机意味着要备案，备案花时间精力也就算了，关键我之前买的域名大概因为是主权国家域名的关系（.li），不让备案。于是就很纠结。最后还是滚去买了阿里云香港。
- [开启 SSL 并使用](https://blog.csdn.net/ithomer/article/details/50433363)，参考文档里的那个 SSL 开启的步骤是有问题的，别看那个。
- 申请免费的 DV 证书。

# 搭建前端
- 在微信公众平台注册，使用了个人主体。下载小程序开发套件。


# Reference
- [微信小程序之PHP服务器搭建](https://blog.csdn.net/longjialin93528/article/details/79727237) 
- [微信小程序文档](https://developers.weixin.qq.com/miniprogram/dev/framework/)
