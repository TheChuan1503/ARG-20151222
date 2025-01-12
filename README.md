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

- **动态是二进制，转为十进制为 `1223→1222`**  

- **视频 `00:08` 处花屏文字 `时间20151222? %←`**  
  ![视频 00:08 处画面](img/1.1.jpg)

- **视频 `00:11` 处花屏文字 `信号传输受阻`**  
  ![视频 00:11 处画面](img/1.2.jpg)

- **视频 `00:17` 处花屏文字 `进行■■协议`**  
  ![视频 00:17 处画面](img/1.3.jpg)

- **视频 `00:23` 处花屏文字**  
  `晚安，迎接你的下一个明天`  
  `晚安，迎接你的下一个昨天`
  ![视频 00:23 处画面](img/1.4.jpg)

### 2. [视频] 20151■■■-Fatal■-error■.mp4
> **动态** 10011000110→1001100010■  
> **BV**1fvrCYAEnd  
> **AV**113798513952833  
> **时间** 2025-01-10 08:01  
> **简介**  
> ``` java
> Exception in thread “main”
>  java.lang.Error: ServerHangWatchdog detected that a single server tick took 60.01 seconds (should be max 0.05)
> ```
- **简介Java异常信息**  
  表示主线程一个tick用时(60.01s)远远超过了正常时间(0.05s)
- **视频中的Linux终端界面**  
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
- **视频背景音为摩斯密码**  
  `.-- .-- .-- .-.-.- -.-. .... .. .--. .-. .- ..-. - .-.-.- - --- .--.`  
  解码得到 `www.chipraft.top`  

- **视频背景隐藏图案**  
  视频背景经过提高曝光后得到SCP反概念部图案
  ![评论图片](img/2.2.jpg)

### 3. [视频] 2015122■-[no signal].mp4
> **动态** 1001100101■→1001100010■■  
> **BV**1f9cnenEaW  
> **AV**113804285379866  
> **时间** 2025-01-10 22:52  
> **简介** `Dkwzobon1gsdr2Dro3Drsbn=`  

- **简介为凯撒加密**
  解密后得到 `Tampered1with2The3Third` (`Tampered  with  The Third` 被The Third篡改)
  ![评论图片](img/3.1.jpg)
- **视频背景音为摩斯密码**  
  `.. -. ... . - -.-. .. -. - .... . -- .. -.. -.. .-.. .`  
  解码得到 `inset c in the middle`  
  结合视频3得到的不完整域名后得到 [`www.chipcraft.top`](http://www.chipcraft.top)  
  
  网站图标![www.chipcraft.top/favicon.ico](http://www.chipcraft.top/favicon.ico)  
  转换为png得到
  ![www.chipcraft.top_icon.jpg](img/www.chipcraft.top_icon.jpg)
  
  内容
  ```
  0sXN/Ln9yKW1xMjLo6y74bG7uf3Ipcv50sXN/KGjw7vT0Ln9yKW1xMjLo6zSsrK71NnTtdPQvavAtA==
  
   
  
  ????????
  
  #404error
  ```
  
  base64 GBK 解码得到  
  `遗忘过去的人，会被过去所遗忘。没有过去的人，也不再拥有将来`  
  
  试图访问不存在的页面会跳转到 `http://www.chipcraft.top/404/?404,http://www.chipcraft.top/xxx`  
  
  页面标题为 `55555`
  
  内容
  ```
  safHuNPD1eK3vcq9tKu13dDFz6K5/cilvavAtL7gwOvMq7OkyM66zszhtb2h9qH2ofYtofah9i2h9qH2ofah9i0xtcTQxc+itry74bG7ofah9qH20KfTpqH2ofah9rDdzdDBy7+0tb3V4rbOtcTIyy2h9qH2ofah9qH2ofah9qH2ofah9qH216HIzqH2udjT2qH2ofah9i2h9qH2LaH2ofah9qH2LTG49szltcSh9qH2
  0sXN/Ln9yKW1xMjLo6y74bG7uf3Ipcv50sXN/KGjw7vT0Ln9yKW1xMjLo6zSsrK71NnTtdPQvavAtA==
  
   
  
  NTU1NTU=
  ```
  
  - 第一行base64 GBK解码后得到  
    `抱歉用这方式传递信息过去将来距离太长任何提到■■■-■■-■■■■-1的信息都会被■■■效应■■■拜托了看到这段的人-■■■■■■■■■■■住任■关于■■■-■■-■■■■-1个体的■■`  
  - 第二行base64 GBK解码后得到  
    `遗忘过去的人，会被过去所遗忘。没有过去的人，也不再拥有将来`  
  - 最后一行base64解码后得到 `55555`
  
  访问 [`http://www.chipcraft.top/55555.png`](http://www.chipcraft.top/55555.png) 后得到一张图片
  ![http://www.chipcraft.top/55555.png](http://www.chipcraft.top/55555.png)  
  图片中隐藏的base64解码后为 `www.chipcraft.top`，无实际作用

### 4. [视频] 20151220_091205_100404.mp4
> **动态** 1001100010■→10011000100  
> **BV**1D5cWeyEet  
> **AV**113804889360362  
> **时间** 2025-01-11 08:54  
> **简介**
> ```
> 30820155020100300d06092a864886f70d01010105000482013f3082013b020100024100a99b1c01199c5e47f82e8a6088e2bf29442fe2654f18eb166c771a9321e2964e8a2a31debf0a1577441a699cab4af6211100bc9df42ad443c3cfa45a5240e4a9020301000102410097b72855d3930cc3543e4d8a0ce8c81721e7b39cec245e26b0dfd9e5c369ed08dba3306163abe1c4f9b730c5e98bb0ec83b2b008079847168cdc3aa4681c2401022100f1c7bde5ea482dbb39b2346aaeb745963eec8a2b5128ab36bfcd3c2c03bd7937022100b394b4ca59bae501829935c4512e675a855dc0b9617850882d6df8f258da011f02202fe3c56c65e458128e920aa9dae37848133c9cfd897cc9b4f576bc6567743f2f0220679053eefa6e791134e2ec8a0a134bd17d6642f5e60b3fce38fcd9fbd157f01b022100de8c0dfb0fcad45e0d856fcbd934be4a1011bb5d2391267791627fcec28e27ef
> ```

- **简介为DER格式的RSA私钥**  
  转为PEM格式得到
  ``` pem
  -----BEGIN PRIVATE KEY-----
  MIIBVQIBADANBgkqhkiG9w0BAQEFAASCAT8wggE7AgEAAkEAqZscARmcXkf4Lopg
  iOK/KUQv4mVPGOsWbHcakyHilk6KKjHevwoVd0QaaZyrSvYhEQC8nfQq1EPDz6Ra
  UkDkqQIDAQABAkEAl7coVdOTDMNUPk2KDOjIFyHns5zsJF4msN/Z5cNp7QjbozBh
  Y6vhxPm3MMXpi7Dsg7KwCAeYRxaM3DqkaBwkAQIhAPHHveXqSC27ObI0aq63RZY+
  7IorUSirNr/NPCwDvXk3AiEAs5S0ylm65QGCmTXEUS5nWoVdwLlheFCILW348lja
  AR8CIC/jxWxl5FgSjpIKqdrjeEgTPJz9iXzJtPV2vGVndD8vAiBnkFPu+m55ETTi
  7IoKE0vRfWZC9eYLP844/Nn70VfwGwIhAN6MDfsPytReDYVvy9k0vkoQEbtdI5Em
  d5Fif87Cjifv
  -----END PRIVATE KEY-----
  ```
  
- **视频背景音为摩斯密码**  
  `.-- . .- .-. . - .... . - .... .. .-. -..`  
  解码得到 `we are the third` (我们是The Third)
  
- **视频种子与视频1种子相同，但是多了告示牌**  
  告示牌内容与视频1相同位置的弹幕相同
  ![视频画面](img/4.1.jpg)

- **视频 `00:02` 处花屏文字 `时间201512220? %←`**
  ![视频00:02处画面](img/4.2.jpg)

- **花屏后玩家发送了消息 `有人在吗？`**
  ![视频00:02处画面2](img/4.3.jpg)

- **视频 `00:03` 处花屏文字 `信号被劫持`**
  ![视频00:03处画面](img/4.4.jpg)
  
- **花屏后玩家了发送消息 `him?`**
  ![视频00:03处画面2](img/4.5.jpg)
  
- **视频 `00:04` 处花屏文字 `需要进行调查`**
  ![视频00:04处画面](img/4.6.jpg)
  
- **视频 `00:10` 处花屏报错与前面的报错相同**
  ![视频00:10处画面](img/4.7.jpg)
  
- **视频 `00:23` 处玩家在告示牌上写 `是你让我...`**  
  随后删除了bian的n，视频变为`[无信号]`
  ![视频00:23处画面](img/4.8.jpg)
- **视频 `00:25` 处无信号界面有短暂轻微的红色闪动**
  ![视频00:25处画面](img/4.9.jpg)
  
### 5. [动态] 1
> **时间** 2025-01-11 13:00  
> **内容** `00:32/02:58→00:54/02:58`

- **推测可能与`【初音ミク】逆模因女孩【ルシノ】`有关**  
  结合作者收藏和动态内容为`【初音ミク】逆模因女孩【ルシノ】`时长
  ![评论图片](img/5.1.jpg)
  ![作者收藏](img/5.2.jpg)
  
### 6. [动态] 1000
> **时间** 2025-01-11 15:09  
> **内容** `Server Access Recovery.`

- **推测是作者到达1000粉丝后开启了关注自动回复**

### 7. [动态] _无标题_
> **时间** 2025-01-12 15:33  
> **内容**  
> `gOr5JnRvM1YrbVch5ag81PknBGKArxIYbv606r7HprRrmD3WA1RB7fzX3jbof8oQn8FSgIdsjSuSB2NCNIXGaw==`
> ![7.1](img/7.1.jpg)

- **内容为RSA密文**  
  经过前面的RSA私钥解密后得到  
  ```
  不要被劫持信号迷惑
  下一则消息在8:00上传
  ```
  
- **告示牌内容为 `是你让我时间`**  
  图片由于滤镜，左边部分已输入的拼音被遮挡，且作者想继续输入w
