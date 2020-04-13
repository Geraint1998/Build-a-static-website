*建站小白的我最近一直在尝试各种建站方案，于是记录下了自己的心得体会*

# 建站的多种方案/[一套完整的建站方案](https://gitee.com/geraint1998/Build-a-static-website/blob/master/%E4%B8%80%E5%A5%97%E5%AE%8C%E6%95%B4%E7%9A%84%E5%BB%BA%E7%AB%99%E6%96%B9%E6%A1%88.md)

**很多小白都想着手搭建自己的网站，我也是，经过一个月的折腾，我摸出了几套建站的方案，**

**可能不是很成熟，还望见谅。**



## 1. 一般方案（新用户100块钱左右能建个一年站）：



* 购买云主机

  

* 购买域名

  

* 域名备案

  （国内备案的概念太混沌了，到底是主机备案，还是域名备案，又或是主机备案）

  

* 写好网站

  

* *在云主机上下载建站助手（可选）*

  

* 将写好的网站数据上传到云主机（推荐**FTP**）

  

* 网站域名解析到云主机的公网IP上

  

  

## 2. Github、Gitee、Coding、Gitlab等项目托管平台二级域名建站（免费）：



* **Github：**（缺点是慢，网上教程很多，我只说下注意点）

  

  （1）网站**项目名称**为 “ **你的用户名** + **github.io** ”

  

  （2）Settings —— Options —— 往下拉到 Github Pages 选择 Choose a theme

  （当然有兴趣的可自己写主题）

  

  （3）基本架构就完成了

  

* **Gitee：**（缺点是自动部署要钱，中文支持不友好）

  

  （1）新建项目，名称随意，选择**公开**（想让人看的话）

  

  （2）在项目里新建 **index.html** (自己写好静态网页的直接上传)

  

  （3）在服务里选 **gitee pages** 

  

  （4）下面就是点橙色按键就完了

  

* **Coding:**（不是打广告，个人觉得UI最舒服，缺点是建项目时的选择题）

  

  （1）新建项目：选 **DevOps** 

  

  （2）名称随意，最好简洁，项目标识点一下，

  选择 Read.me 初始化，然后默认

  

  （3）构建与部署里选**静态网页**

  

  （4）名称自定，点击完成

  

  （5）然后自己写一个静态网页程序放在项目里测试打开

  

  （6）**注：**网址在**构建与部署——静态网页下**

  

* **Gitlab:**（没试过，道理差不多）





## 3. 自助建站网站二级域名建站：（有免费有收费，看需求，缺点是有平台条幅）



* wix（台湾）：缺点是速度慢，有平台条幅，繁体改不了，优点是易操作，UI好看

  

* 建个站（国内）

  

* 意派Coolsite360（国内）

  

* 其它（网上搜自助建站）





## 4. 网站托管：（好坏未知，还没尝试）



* name.com

  

* 其它





## 5. ftp建站：



* 最简单是是租服务器，因为有**公网IP**，然后开启 **IIS** 和 **FTP** 服务，在 **IIS** 里建 **FTP站点**，

  IP地址就填**公网IP**，然后输入IP地址直连

  

* 自己的电脑多一个把FTP映射到外网据体的[这篇文章](http://www.nat123.com/Pages_8_261.jsp)有讲，软件不一定用里面说的，

  类似的软件也可以百度，比如内网穿透，很多人喜欢用花生壳

  

* FTP建站主要用于资源共享，网站UI比较简陋，也许有大神会吧





## 6.各种云的对象存储产品建站：（其他没试过，腾讯云可以）



* 打开你自己新建的存储桶（腾讯云为例）

  

* 选择**基础配置**

  

* 下拉找到静态网站

  

* 编辑——开启（可以选择强制HTTPS），保存，

  注意记住**访问节点**

  

* 点击**权限管理**

  

* 选择**公有读私有写**

  

* 本地新建 **index.html** (与**静态网站**设置里的**索引文档名**相同)

  

* 上传到存储桶里，点击**详情**

  

* **对象访问权限**选择**公有读私有写**，这里的**对象地址**也可以用来访问，

  但是建议用前面记住的**访问节点**





## 7. 自建服务器托管网站：（最麻烦的，新手的我表示不会）
