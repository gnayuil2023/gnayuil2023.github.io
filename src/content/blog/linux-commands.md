---
title: "Linux 常用命令"
description: "Migrated from original blog"
pubDate: "2023-07-10T03:05:21.000Z"
heroImage: "/assets/blog-placeholder-3.jpg"
---

### < id="常用命令整理">常用命令整理>

查看当前文件目录下的所有文件ls

查看根目录下的文件ls /

查看根目录的详细属性ls -ld /

查看当前文件目录下所有文件的详细信息# 可查看文件的文件名、创建时间、操作权限等信息
ll

查看某个文件的内容# fileName为文件名
cat fileName

清空终端上的内容clear

进入某个文件夹下# ~/.ssh 表示文件夹的路径
cd ~/.ssh

创建文件目录# test 表示文件目录名称
mkdir test

创建多级文件目录# test/data/fyt 表示文件目录
mkdir -p test/data/fyt

刪除文件目录# test 表示文件目录名称
rmdir test

创建文件# a.md 表示需要创建的文件
touch test.md

回到上一级目录cd ..

回到根目录cd ~

查看本机的ip地址ifconfig

清屏clear

安装 wgetyum -y install wget

安装网络工具包yum install net-tools -y 

查看当前工作目录pwd

查看命令行中操作的历史记录history

将文件传送到 Linux 服务器上# hi.c 需要上传到 Linux 服务器上的文件
# root 登录 Linux 服务器的用户名
# 192.168.50.23 Linux 服务器的 ip 地址
scp hi.c root@192.168.50.23/root

解压文件# node-v12.4.0.tar.xz 要解压的文件
tar -xvf node-v12.4.0.tar.xz

使用 rsa 算法生成秘钥ssh-keygen -t rsa

在终端中查看生成的公钥cat ~/.ssh/id_rsa.pub

在 vim 中查看生成的公钥vim  ~/.ssh/id_rsa.pub

检测是否和 github 建立连接ssh -T git@github.com

退出 vim:wq

关闭 Linux 服务器shutdown

base64 加密echo "hello world" | base64

base64 解密echo "aGVsbG8gd29ybGQK" | base64 -d

查看文件所在的目录# 查看 redis 所在的目录
whereis redis

进入 redis 数据库操作界面redis-cli

登录 redis 数据库# 009527 为登录 redis 数据库的密码
auth 009527

进入 redis 下的某个数据库# 8 表示进入 redis 下的第 8 个数据库
select 8

查看 redis 数据库下的所有数据keys *

删除 redis 数据库中的数据flushall
