# PDA-订单拣货

<font style="color:#374051;">pda的订单拣货只能单笔提交下一环节，具体操作步骤如下：</font>

<font style="color:#374051;">1.点击订单拣货按钮，用户可见如图界面，通过输入、扫描系统单号或运单号操作需拣货订单。</font>

![1587980621952-2a80286d-c0e2-4652-865f-05a146acbfe2.jpeg](./img/mRkkbyAvvBzOViyf/1587980621952-2a80286d-c0e2-4652-865f-05a146acbfe2-994497.jpeg)

<font style="color:#374051;">2.选择订单后，用户可以根据商品显示的库位进行取货。扫描库位，相应订单需要此库位上的商品就会标记已完成。</font>

![1587980622132-8412a224-fa6e-4818-b940-b2eaa76127ab.jpeg](./img/mRkkbyAvvBzOViyf/1587980622132-8412a224-fa6e-4818-b940-b2eaa76127ab-500754.jpeg)

<font style="color:#374051;">点击商品数量，弹窗可修改数量，点击完成即可。</font>

![1587980622325-6276fee0-83b8-443b-ba99-fe9bbc520f01.jpeg](./img/mRkkbyAvvBzOViyf/1587980622325-6276fee0-83b8-443b-ba99-fe9bbc520f01-339014.jpeg)

<font style="color:#374051;">支持右上角查看拣货进度，扫描商品条码，拣货进度根据扫描商品的数量更新，扫描箱条码时，拣货进度增加的是箱内库存的数量；</font>

![1587980622486-fc48ad7a-3059-4eb8-8d3a-697619a9f560.jpeg](./img/mRkkbyAvvBzOViyf/1587980622486-fc48ad7a-3059-4eb8-8d3a-697619a9f560-541012.jpeg)

<font style="color:#374051;">3.所有的商品行都为已完成，则会自动弹窗提交，点击确认即可。</font>

![1587980622675-045803b2-6a8c-4c36-9e35-04065db41723.jpeg](./img/mRkkbyAvvBzOViyf/1587980622675-045803b2-6a8c-4c36-9e35-04065db41723-489791.jpeg)

<font style="color:#374051;">4.</font>开启按库区接力拣货，一个库区明细拣货完成后，提示库区拣货已完成是否提交，确认提交后生成接力拣货任务。下个库区拣货直接扫描运单号领取接力拣货任务。

![1597196013307-8cca493f-4dec-4fa3-85b9-0b6c19908c26.png](./img/mRkkbyAvvBzOViyf/1597196013307-8cca493f-4dec-4fa3-85b9-0b6c19908c26-751101.png)

<font style="color:#000000;">提示</font>

<font style="color:#000000;">1. </font><font style="color:#000000;">如开启了</font><font style="color:#000000;">PDA</font><font style="color:#000000;">拣货检验商品条码配置，则根据配置的结果，拣货时进行库位或商品条码扫描。</font>

<font style="color:#000000;">2.序列号商品，扫描商品条码后跳转序列号录入界面，商品数量不可编辑。</font><font style="color:#000000;"> </font>

<font style="color:#000000;">3.</font><font style="color:#000000;">一次性录入序列号，后台开关</font><font style="color:#000000;">开启保留区间截取，示例：</font>

<font style="color:#000000;">解析规则：保留区间截取，品牌：新增的品牌，保留区间截取第6到18位，条码长度范围为从0-21</font>

<font style="color:#000000;">商品A系统中商品条码69200811001-新增的品牌-序列号商品</font>

<font style="color:#000000;">商品B系统中商品条码69200811002-新增的品牌-非序列号商品</font>

<font style="color:#000000;">收货入库页面扫描条码</font><font style="color:#000000;">1234569200811001001，</font><font style="color:#000000;">匹配到了商品A且录入序列号</font><font style="color:#000000;">1234569200811001001</font><font style="color:#000000;">。</font>

<font style="color:#000000;">收货入库页面扫描条码1234569200811002001，匹配到了商品B不录入序列号。</font>

4.若商品为序列号商品且序列号登记环节在拣货，即商品需录入序列号，序列号支持修改。

![1720072027467-a77c93f1-a8ae-481c-992b-260dbfdc1eb1.png](./img/mRkkbyAvvBzOViyf/1720072027467-a77c93f1-a8ae-481c-992b-260dbfdc1eb1-098023.png)

点击修改输入序列号若符合，则确认后修改成功。

注：修改序列号不会再次扣减库存。

![1720072136635-b587ce55-72b0-404e-b2cc-5cbd74acfd90.png](./img/mRkkbyAvvBzOViyf/1720072136635-b587ce55-72b0-404e-b2cc-5cbd74acfd90-512016.png)

                   

 



> 更新: 2024-07-04 13:49:41  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/bwipfoa3yuv0g7zh>