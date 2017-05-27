# apt彻底删除nginx

在ubuntu中nginx又多个软件，

```
sudo apt-get --purge remove nginx  
sudo apt-get autoremove  
dpkg --get-selections|grep nginx 
```
