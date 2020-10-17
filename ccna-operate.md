# CCNA 主機操作筆記
![](https://i.imgur.com/5AJfuzI.png)

----

進入特權(#)
```
en
```
進入全域設定
```
config t
```

退到前一個層級
```
exit
```
查看設定檔
```
# show run
```
設定交換器名稱
```
(config)# hostname <name>
```
設定交換器IP
```
(config)# interface vlan(interface) 1
(config-if)# ip address <ip> <subnet mask>
(config-if)# no shutdown
```
設定 MOTD 標語 
```
(config)# banner motd "This is banner motd!"
```
最外層密碼設定
```
(config)# line <console(線路名稱)> 0
(config)# password <password>
(config)# login
```
特權密碼
```
(config)# enable password c1$c0
```
加密密碼 (會覆蓋上者之密碼)
```
(config)# enable secret <password>
```
明文密碼加密
```
(config)# service password-encryption
```
設定檔儲存到 NVRAM
```
# copy running-config startup-config
```