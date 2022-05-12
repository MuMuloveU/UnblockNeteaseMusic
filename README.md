# 利用UnblockNeteaseMusic解锁网易云灰色歌曲

#### 你只需要准备一台云服务器 

```
为什么会有这个项目？我这个项目和原项目有什么区别？
原项目链接:
https://github.com/meng-chuan/Unlock-netease-cloud-music
原项目的安装教程过于陈旧，不在适用，耽误了我很多时间。
我仅仅修改了原项目的两个地方 
Unlock-netease-cloud-music/src/app.js 19行将8080修改为52000
Unlock-netease-cloud-music/src/cli.js 4行后添加一行 port:"52000:52001",

```



## 0x01 为你的服务器安装centos 或者 Ubuntu 系统

## 0x02 安装宝塔面板 

在这个网页寻找关于安装的帮助      https://www.bt.cn/new/download.html

## 0x03安装PM2管理器

![image-20220512140839204](https://cdn.jsdelivr.net/gh/MuMuloveU/tuchuang/202205121408325.png)

## 0x04 把这个项目上传到服务器

你可能需要先克隆到本地

git clone https://github.com/MuMuloveU/UnblockNeteaseMusic

![image-20220512141335757](https://cdn.jsdelivr.net/gh/MuMuloveU/tuchuang/202205121413841.png)

## 0x05在PM2管理器中添加并运行本项目

启动文件选择src目录下的 app.js

内存上限设置为200MB

运行用户选择root

![image-20220512143516807](https://cdn.jsdelivr.net/gh/MuMuloveU/tuchuang/202205121435892.png)

## 0x06 放行端口

![image-20220512142126290](https://cdn.jsdelivr.net/gh/MuMuloveU/tuchuang/202205121421337.png)

网易云音乐代理设置 

ip地址 你的服务器ip 

端口   52000

![image-20220512152755288](https://cdn.jsdelivr.net/gh/MuMuloveU/tuchuang/202205121527355.png)
