# rpi_tracked
记录一次树莓派被攻击


 来自 俄罗斯 和 江苏镇江的  root 尝试登陆

![1](https://dn-shimo-image.qbox.me/zt8HPnUvjogzqXJU.png)



![13](https://dn-shimo-image.qbox.me/KQ4aLFmfYJoltnnG.png)



大量 auth.log日志记录发现 ，被入侵后 好像给我生成了某些cron脚本，导致频繁执行，
在删掉某用户后，提示不能找到什么云云。
![2](https://dn-shimo-image.qbox.me/I7H3zU83OQUcYIcy.png!thumbnail)
![3](https://dn-shimo-image.qbox.me/50nKPo024uASlo1l.png)
被 fail2ban记录禁止的 来自 美国vps的攻击尝试。

![11](https://dn-shimo-image.qbox.me/88HCllAhcPYHCtZy.png)

原来 是给我的 cron写入一个每时每刻每分每秒都在执行的任务，。。。。。。。
![10](https://dn-shimo-image.qbox.me/tom2B8mF14US6oyx.png)
特么的 服。。。。

 date:  2016年 04月 02日 星期六 22:30:33 CST
 ![16](https://dn-shimo-image.qbox.me/ljiJ4HmcL1E4UulJ.png)
 又开始了。
 ![17](https://dn-shimo-image.qbox.me/2NeNOKhHJWgV5wkZ.png)
