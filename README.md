# 过YD443端口

## 一、一键安装命令：
```
wget https://raw.githubusercontent.com/xcazt/ydpass/main/gyd && chmod 744 /root/gyd
```
## 二、后台运行

### 1、添加OUTPUT
```
iptables -I OUTPUT -p tcp --sport 443 -j NFQUEUE --queue-num 443 --queue-bypass
```
### 2、运行
```
./gyd -q 443 -w 20 -c 10
```
## 默认秘钥：G3HD-MFYQ-8H7J-450Q

本文件介绍内容只用于学习交流，若有侵权，请联系删除！
