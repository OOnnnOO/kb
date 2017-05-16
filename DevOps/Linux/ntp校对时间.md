# ntp校对时间

Debian系统安装NTP包

```
apt-get install ntpdate
```

RenHat系 安装NTP包
```
yum install ntp
```

校准命令：

```
ntpdate cn.pool.ntp.org
```

加入定时任务

```
00 12 * * * /sbin/ntpdate cn.pool.ntp.org
```
