# WMS-微信小店代发（供货商）

### 背景
2025年12月1日起，微信官方平台逐步调整跨店铺代打业务的规范性。详情可点击查看[平台公告](https://store.weixin.qq.com/chengzhang/webdoc/wiki/8469/5f00c2182495bdfd/growth_center_platform_notice)。其中**<font style="color:rgba(0, 0, 0, 0.9);">当且仅当「订单所属店铺」与「代打单店铺」具备经营主体关系时，双方店铺方可使用</font>****<font style="color:#DF2A3F;">原代打功能</font>****<font style="color:rgba(0, 0, 0, 0.9);">。否则只能使用「</font>****<font style="color:#DF2A3F;">官方代发工具</font>****<font style="color:rgba(0, 0, 0, 0.9);">」</font>**

本次功能即为官方代发工具（微信小店供货商代发）

万里牛WMS供货商代发，**订购100元退80元**，平台技术服务费20元

### 影响范围
本次微信官方调整将将在12月逐步启动，届时将影响WMS现有业务开展，影响范围为

**使用某一视频号小店（微信小店）订购电子面单替其他无经营关联店铺进行取号打单的用户**

****

### 建议改造方式
1.向自有多店铺商家，向平台证明代取号店铺和取号店铺间具备同一经营主体关系

2.云仓经营方，自行申请微信小店供货商身份，并进行绑定代打店铺（详情可见[微信小店「供货商关联商家」操作指引](https://store.weixin.qq.com/chengzhang/webdoc/wiki/8205/ea21caa54d1d14d8/growth_center_manual_for_supplier)）



### 供货商方案示意
![画板](./img/VCAQTB_zoJKq9IqM/1784254621304-a430eef6-99ad-453d-b220-84ad27439853-717891.jpeg)

### 微信小店代发系统操作方式
#### 店铺授权




订购应用：万里牛WMS供货商代发，**订购100元退80元**，平台技术服务费20元（20%收取）

![1766040174789-433e9922-ecf9-4a5f-ac38-7e898474c81f.png](./img/VCAQTB_zoJKq9IqM/1766040174789-433e9922-ecf9-4a5f-ac38-7e898474c81f-519789.png)

新增店铺或将ERP推送的店铺进行授权

![1765265883622-b74ae4c2-f183-4f2d-925a-261582135680.png](./img/VCAQTB_zoJKq9IqM/1765265883622-b74ae4c2-f183-4f2d-925a-261582135680-906065.png)

填写正确的供应商ID,特别注意当小店既是视频号微信小店身份又是供货商身份时必须填写对应正确的ID ![1766039495871-915ad520-cb4c-4925-82bd-4e695cbc73e5.png](./img/VCAQTB_zoJKq9IqM/1766039495871-915ad520-cb4c-4925-82bd-4e695cbc73e5-577176.png)

参考位置

![1766039400111-c1a824e6-de43-475c-bc50-c9812cac41d9.png](./img/VCAQTB_zoJKq9IqM/1766039400111-c1a824e6-de43-475c-bc50-c9812cac41d9-695822.png)

#### 开通电子面单
新增承运商后或已有承运商启用电子面单接口，选择微信小店供货商接口

![1765266055657-7a88390d-8a8a-49e5-9eb1-5e15bf7a6340.png](./img/VCAQTB_zoJKq9IqM/1765266055657-7a88390d-8a8a-49e5-9eb1-5e15bf7a6340-818821.png)

启用后，配置店铺、网点相关信息，其余操作同视频号电子面单一致

![1765266137843-b1c76a47-3bd3-4fb1-9177-7a4f543e7b5a.png](./img/VCAQTB_zoJKq9IqM/1765266137843-b1c76a47-3bd3-4fb1-9177-7a4f543e7b5a-195452.png)



#### 单据查看
该类供货商代发单区别于正常的视频号（微信小店）订单，在系统中的店铺类型为微信小店供应商。![1765266356023-231bc2dc-ca85-4da4-8dab-9c0937ae64c4.png](./img/VCAQTB_zoJKq9IqM/1765266356023-231bc2dc-ca85-4da4-8dab-9c0937ae64c4-899934.png)

#### 业务识别条件
供货商代发单识别：

<font style="color:rgb(0, 0, 0);">平台来源编码为：WXXDDF 微信小店代发</font>  
<font style="color:rgb(0, 0, 0);">代发订单商品信息：request->orderLines->orderLine->extCode 平台商品编码</font>

<font style="color:rgb(0, 0, 0);"></font>

<font style="color:rgb(0, 0, 0);">供货商代发方案几点注意事项：</font>

<font style="color:rgb(0, 0, 0);">1.供货商店铺建立后需要去平台获取代发单，而非处理销售店铺的订单</font>

<font style="color:rgb(0, 0, 0);">2.供货商店铺只可给自己店铺的代发单申请电子面单，其余都不行。</font>

<font style="color:rgb(0, 0, 0);">3.供货商小店的供应商ID必须填当前店铺的供应商ID</font>



> 更新: 2026-07-17 10:21:21  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/hzmsryuw1getafah>