# WMS-京东全渠道京配电子面单（京东零售）

### 业务介绍
京东零售源头直发业务改为由京东快递提供承运支持，需要单独获取全渠道京配电子面单发货

### 操作说明


<font style="color:rgb(60, 67, 83);">WMS识别京东零售订单：当sourcePlatformCode 订单来源编码为JD，request—>deliveryOrder—>extendProps—>delivery_mode，delivery_mode值为12，识别此订单为全渠道京配订单。</font>

#### 京东店铺后台配置
[查看详细配置流程](https://joyspace.jd.com/pages/8H1nV2WWjsymo21ha2gL)



#### 店铺授权
选择京东平台登录进行授权，全渠道京配业务不支持跨店铺获取面单，故每一个发货店铺都需要授权

![1757488173048-bba07531-20df-44c1-951c-436b185a7603.png](./img/f5CtjyY5ZqWTkTf9/1757488173048-bba07531-20df-44c1-951c-436b185a7603-126848.png)

#### 开通电子面单
授权成功后，选择京东快递，找到全渠道直连京配电子面单接口

![1757487707968-59dc66ef-a0d2-4915-95e0-d567e2efb3a2.png](./img/f5CtjyY5ZqWTkTf9/1757487707968-59dc66ef-a0d2-4915-95e0-d567e2efb3a2-380922.png)

填写authKey（需联系京东采销人员提供）和青龙编码

![1757488010189-ee1c4c1b-bec2-40d0-ad89-7d47a1e3b8c4.png](./img/f5CtjyY5ZqWTkTf9/1757488010189-ee1c4c1b-bec2-40d0-ad89-7d47a1e3b8c4-308057.png)

![1757487896850-d3c58b1a-d1fe-4136-8c9b-020ef8f648b1.png](./img/f5CtjyY5ZqWTkTf9/1757487896850-d3c58b1a-d1fe-4136-8c9b-020ef8f648b1-710648.png)

选择对应的产品类型即可

![1757488282838-6b1094c2-d4e9-4429-aa95-33fd75ec39a6.png](./img/f5CtjyY5ZqWTkTf9/1757488282838-6b1094c2-d4e9-4429-aa95-33fd75ec39a6-472476.png)



> 更新: 2025-11-27 11:48:32  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/vf3z5qrakahh5nrv>