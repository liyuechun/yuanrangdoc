# 绑定独立域名

## 一、域名备案（ICP）

首先需要先申请一个域名。有了域名之后，需要在腾讯云上进行备案。**注意，一定是腾讯云。**如果在阿里云备案过了，也要在腾讯云备案，但是备案审核会稍微快一些。

备案时间一般几天到**20天**不等（根据经验，12天左右）。

腾讯云网址：[https://cloud.tencent.com/](https://cloud.tencent.com/)

 ![](https://file.liyuechun.com/AgAABdffSvfNS8fG6hVBu4c7NaYOfONt.png?w=1896&h=1110)         



按照要求上传证件，一步一步进行即可。

 ![](https://file.liyuechun.com/AgAABdffSvfCe2kZke1LL7_cySeNBqsw.png?w=3068&h=1906)         



注意：备案域名时会要求绑定云服务器，如果您之前有云服务器直接绑定即可。如果没有，建议您买个最便宜的就行。比如轻量级云服务器，时长不要少3个月，这是腾讯云建议的。备案成功后，可以退掉服务器。（还能退点钱😁）

推荐个相对便宜点的轻量级服务器：https://cloud.tencent.com/product/lighthouse

![](https://file.liyuechun.com/AgAABdffSvdKSONf0KRAxbdl2XDtnp1a.png?w=2360&h=1518)

如果这个服务器只是为了备案，您不做其他用途，那镜像这里看着选。

![](https://file.liyuechun.com/AgAABdffSved4sEdUAJLIL7Mf2KQJNKF.png?w=2338&h=1494)

当域名备案通过，您记得来腾讯云这里退一下服务。可以退回一部分钱。

## 二、申请SSL证书

备案通过后，需要申请SSL证书。同样也是在腾讯云上。

![](https://file.liyuechun.com/AgAABdffSvdW2gYT2SBIjJQQaOQw7u7G.png?w=1904&h=1184)         



申请免费 SSL 证书。

![](https://file.liyuechun.com/AgAABdffSvcwyhPMgpJLvoY9vdIBVtMH.png?w=2912&h=1406)         



然后填写信息提交即可。

![](https://file.liyuechun.com/AgAABdffSvd5n0a2CilKeKvZ7a9P393-.png?w=2504&h=1350)    



##   三、     **解析域名**

提交申请后，会让你添加一条域名解析记录。你要回到购买域名的平台去进行添加。（阿里云买域名就去阿里云添加，腾讯云买就腾讯云添加，百度云买就百度云添加）。

此处添加两条解析记录。一条是腾讯云指定的，为了 SSL 认证。第二条是为了解析元壤店铺地址。原理都是一样，就是配置的内容不一样。

**第一条解析记录：**

按照腾讯云的要求，填入主机记录，记录类型，记录值即可。

![](https://file.liyuechun.com/AgAABdffSvd5RNJ0FY1AHZTIIAgudC98.png?w=2946&h=1232)



**第二条解析记录：**

这个是用来解析您店铺地址的。和上面申请 SSL 证书的时候，添加的解析记录是一回事儿。只不过配置的内容是您的元壤店铺后台地址。

这里以阿里云为例。首先在控制台找到域名这一项：

​                  ![](https://file.liyuechun.com/AgAABdffSvc2wS_s_-VPcp0Q9ary-15J.png?w=2414&h=1064)         



点开域名列表：

​                  ![](https://file.liyuechun.com/AgAABdffSvcxL_QFQQ9JWrAWpG309gaE.png?w=2856&h=986)         



在购买的域名后面，点击解析，进到解析设置页，点击添加记录：

​                  ![](https://file.liyuechun.com/AgAABdffSvfAiJ2QJ7tNJJi8zltut27V.png?w=2872&h=994)         



然后按照要求填入信息：

​                  ![](https://file.liyuechun.com/AgAABdffSve9mPnB2X1ERrNerB4q1Mj-.jpeg?w=1540&h=1480)         



稍等一下下就生效了。



然后等待 SSL 审核。

![](https://file.liyuechun.com/AgAABdffSvf-nQN4SHpINIBO8oa0Lvek.png?w=3058&h=1270)



这个也需要一点审核时间。然后您将申请下来的 SSL 证书文件，发送给元壤的工作人员，元壤这边会将域名和店铺进行绑定。

下载证书的时候选择Nginx下载即可。

![](https://file.liyuechun.com/AgAABdffSvdIMuseXCNHD5UND0sHeaYT.png?w=1634&h=1518)
