# ARG-20151222

## 放在前面
### 关于此ARG
- 此ARG围绕bilibili@**bili_20151222** (UID: 3546831258651103)展开
- 与此ARG相关的域名只有 `www.chipcraft.top`，其他子域及其他域名均与本ARG无关
- 此ARG与SCP基金会强关联
### 什么是ARG?
- ARG是一种跨媒体、即时、不可逆的游戏，通常为解密类游戏
### 关于此文档
- 部分素材来源于 bili_20151222 的QQ讨论群和 [(补档)bili_2015 arg解谜进度公示（1.11期） - 哔哩哔哩](https://m.bilibili.com/opus/1021255386614726657)
- 解读内容由群友和bilibili网友共同得出

## 解析
### 0. 作者主页介绍
作者主页介绍原文  
`utrUwsrHt/G6v73Qo78=`  

base64 GBK 解码得  
`黑月是否嚎叫？` (SCP基金会系列作品中的常见暗号)  

黑月是否嚎叫？（Does the black moon howl?）是网络共笔怪谈体系《SCP基金会》中的一句常见暗语。最早出现于SCP-256中

向作者私信 `不，迅捷的棕狐狸跃过懒惰的狗`
![私信作者](img/0.1.jpg)
### 1. [视频] 20151222_060439_071658.mp4
> **动态** 10011000111→10011000110  
> **BV**1eEr6Y7EGS  
> **AV**113796366471023  
> **时间** 2025-01-09 11:55  
> **简介** `［no signal］`

- 动态是二进制，转为十进制为 `1223→1222`

- 视频 `00:08` 处花屏文字 `时间20151222? %←`
  ![视频 00:08 处画面](img/1.1.jpg)

- 视频 `00:11` 处花屏文字 `信号传输受阻`
  ![视频 00:11 处画面](img/1.2.jpg)

- 视频 `00:17` 处花屏文字 `进行■■协议`
  ![视频 00:17 处画面](img/1.3.jpg)

- 视频 `00:23` 处花屏文字  
  `晚安，迎接你的下一个明天`  
  `晚安，迎接你的下一个昨天`
  ![视频 00:23 处画面](img/1.4.jpg)

### 2. [视频] 20151■■■-Fatal■-error■.mp4
> **动态** 10011000110→1001100010■  
> **BV**1fvrCYAEnd  
> **AV**113798513952833  
> **时间** 2025-01-10 08:01

**简介**
``` java
Exception in thread “main”
 java.lang.Error: ServerHangWatchdog detected that a single server tick took 60.01 seconds (should be max 0.05)
```
- 简介是Java异常信息，表示主线程一个tick用时(60.01s)远远超过了正常时间(0.05s)
- 视频中的Linux终端界面
  ![视频画面](img/2.1.jpg)
  内容为
    ``` bash
    [root@localhost ~]# pwd
    /home/s■ps/antimeme/2015
    [root@localhost ~]# cd /122■/
    [root@localhost ~/122■]# ./■■■2■■.sh → 201■■2■■
    Loading------------->
    ```
  解析:
  1. 打印当前目录
  2. 进入 `/122■/` 目录
  3. 执行脚本 `■■■2■■.sh` ( `→202■■2■■` 的作用未知)
  4. 脚本输出 `Loading------------->` 表示加载中  
- 视频背景音为摩斯密码  
  `.-- .-- .-- .-.-.- -.-. .... .. .--. -.-. .-. .- ..-. - .-.-.- - --- .--.`  
  
  解码得到 [`www.chipcraft.top`](http://www.chipcraft.top)  
  
  网站源码
  ``` html
  <!DOCTYPE html>
  <html>
  <head>
  <meta charset="utf-8">
  <title>?????</title>
  </head>
  <body>
  
  <p>0sXN/Ln9yKW1xMjLo6y74bG7uf3Ipcv50sXN/KGjw7vT0Ln9yKW1xMjLo6zSsrK71NnTtdPQvavAtA==</p>
  <p>&nbsp;</p>
  <p>????????</p>
  #404error
  </body>
  </html>
  ```
  内容
  ```
  0sXN/Ln9yKW1xMjLo6y74bG7uf3Ipcv50sXN/KGjw7vT0Ln9yKW1xMjLo6zSsrK71NnTtdPQvavAtA==
  
   
  
  ????????
  
  #404error
  ```
  
  base64 GBK 解码得到  
  `遗忘过去的人，会被过去所遗忘。没有过去的人，也不再拥有将来`

- 视频背景隐藏图案  
  视频背景经过提高曝光后得到SCP反概念部图案
  ![评论图片](img/2.2.jpg)