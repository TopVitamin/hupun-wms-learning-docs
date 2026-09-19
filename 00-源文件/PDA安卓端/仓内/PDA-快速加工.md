# PDA-快速加工

<font style="color:#374051;">业务场景：仓库加工作业频繁，随意没有明细计划性，如果由ERP发起加工单就较为麻烦，由PDA根据ERP的BOM规则自动对应成品和原料进行反算，然后生成加工单同步给ERP。</font>

**<font style="color:#374051;">目前仅支持万里牛ERP对应对接使用</font>**

**<font style="color:#374051;"></font>**

#### <font style="color:#374051;">01.</font><font style="color:#374051;">组合加工</font>
<font style="color:#374051;">操作步骤如下：</font>

<font style="color:#374051;">1.</font><font style="color:#374051;">点击快速加工图标，跳转如图页面，加工方式默认组合加工，在底部的扫描框录入成品商品的条码</font>

![1587980962381-08f0ff00-0059-4989-a2c4-cf589da37830.jpeg](./img/dUAAYN31s4IX1er4/1587980962381-08f0ff00-0059-4989-a2c4-cf589da37830-392160.jpeg)

<font style="color:#374051;">2.</font><font style="color:#374051;">扫描录入成品商品的条码后，根据</font><font style="color:#374051;">ERP</font><font style="color:#374051;">的</font><font style="color:#374051;">BOM</font><font style="color:#374051;">规格带出成品、原料商品以及配比数，如图所示：</font>

![1587980962574-72e31ea9-7327-4226-ad6a-e4eb3938e8ff.jpeg](./img/dUAAYN31s4IX1er4/1587980962574-72e31ea9-7327-4226-ad6a-e4eb3938e8ff-036940.jpeg)

<font style="color:#374051;">3.</font><font style="color:#374051;">点击成品商品的数量，可以编辑修改商品数量，修改后，原料商品的数据根据配比数自动增减，此处原料商品数量不支持修改。</font>

![1587980962789-247e11d2-4886-4f85-a1fa-3d57a4ffefe2.jpeg](./img/dUAAYN31s4IX1er4/1587980962789-247e11d2-4886-4f85-a1fa-3d57a4ffefe2-968128.jpeg)

<font style="color:#374051;">4.</font><font style="color:#374051;">添加完成品，编辑完商品数量后，点击下一步跳转到加工确认页面，系统根据</font><font style="color:#374051;">PC</font><font style="color:#374051;">端设置的加工单配置指定的原料商品锁定范围自动锁定原料库位，锁定失败后，点击</font>![1587980962936-c7a7b780-1f07-4efa-a055-081ea3c657df.jpeg](./img/dUAAYN31s4IX1er4/1587980962936-c7a7b780-1f07-4efa-a055-081ea3c657df-928526.jpeg)<font style="color:#374051;">图标在全仓范围内锁库，底部的库位扫描框扫描录入库位编码，加工成品的目标库位自动填充，如图所示：</font>

![1587980963155-060a4a4a-375b-4513-91e2-7dc52e77b6ea.jpeg](./img/dUAAYN31s4IX1er4/1587980963155-060a4a4a-375b-4513-91e2-7dc52e77b6ea-686657.jpeg)

<font style="color:#374051;">5.</font><font style="color:#374051;">点击提交，加工完成，</font><font style="color:#374051;">PC</font><font style="color:#374051;">端仓内加工自动生成组合加工单并通知</font><font style="color:#374051;">erp</font><font style="color:#374051;">，通知</font><font style="color:#374051;">erp</font><font style="color:#374051;">超时跳转快速加工异常页面，点击重试，重新推送</font><font style="color:#374051;">erp</font><font style="color:#374051;">，点击跳过，回到快速加工页面，继续快速加工操作，如图所示</font><font style="color:#374051;">:</font>

![1587980963324-fc98a061-f41b-4268-8df3-d5f2045b4dbe.jpeg](./img/dUAAYN31s4IX1er4/1587980963324-fc98a061-f41b-4268-8df3-d5f2045b4dbe-183476.jpeg)

#### <font style="color:#374051;">02.</font><font style="color:#374051;">拆分加工</font>
<font style="color:#374051;"> </font>

<font style="color:#374051;">1.</font><font style="color:#374051;">在快速加工页面将作业方式修改为拆分加工，扫描录入成品商品的条码，根据</font><font style="color:#374051;">ERP</font><font style="color:#374051;">的</font><font style="color:#374051;">BOM</font><font style="color:#374051;">规格带出成品、原料商品以及配比数，如图所示：</font>

![1587980963558-d7124689-73b7-4bb6-be67-3bf991a1eef7.jpeg](./img/dUAAYN31s4IX1er4/1587980963558-d7124689-73b7-4bb6-be67-3bf991a1eef7-079551.jpeg)

<font style="color:#374051;">2.</font><font style="color:#374051;">点击成品商品的数量，可以编辑修改商品数量，修改后，原料商品的数据根据配比数自动增减，此处原料商品数量不支持修改。</font>

![1587980963720-07710f42-baff-45b7-88f2-730247c1222b.jpeg](./img/dUAAYN31s4IX1er4/1587980963720-07710f42-baff-45b7-88f2-730247c1222b-884497.jpeg)

<font style="color:#374051;">3.</font><font style="color:#374051;">添加完成品，编辑完商品数量后，点击下一步跳转到加工确认页面，系统根据</font><font style="color:#374051;">PC</font><font style="color:#374051;">端设置的加工单配置指定的原料商品锁定范围自动锁定</font><font style="color:#374051;">BOM</font><font style="color:#374051;">规则中成品商品的库位，锁定失败后，点击</font>![1587980962936-c7a7b780-1f07-4efa-a055-081ea3c657df.jpeg](./img/dUAAYN31s4IX1er4/1587980962936-c7a7b780-1f07-4efa-a055-081ea3c657df-928526.jpeg)<font style="color:#374051;">图标在全仓范围内锁库，底部的库位扫描框扫描录入库位编码，</font><font style="color:#374051;">BOM</font><font style="color:#374051;">中原料的库位由上到下依次填充，如图所示：</font>

![1587980963895-a9c91f61-0e1e-4266-9ae5-a97bd28e3511.jpeg](./img/dUAAYN31s4IX1er4/1587980963895-a9c91f61-0e1e-4266-9ae5-a97bd28e3511-904278.jpeg)

<font style="color:#374051;">4.</font><font style="color:#374051;">点击提交，加工完成，</font><font style="color:#374051;">PC</font><font style="color:#374051;">端仓内加工自动生成拆分加工单并通知</font><font style="color:#374051;">erp</font><font style="color:#374051;">。</font>

<font style="color:#374051;">提示：</font>

1.<font style="color:#374051;">快速加工为后台开关，需要找</font><font style="color:#374051;">wms</font><font style="color:#374051;">技术开启，仅对万里牛</font><font style="color:#374051;">ERP</font><font style="color:#374051;">直连有效；</font>

2.<font style="color:#374051;">快速加工扫描的商品要实现在</font><font style="color:#374051;">ERP</font><font style="color:#374051;">进行仓储商品同步；</font>

<font style="color:#374051;">3.快速加工仅支持普通商品，</font><font style="color:#374051;">BOM</font><font style="color:#374051;">规则中成品为序列号商品、生产批次商品的扫描报错；</font>

<font style="color:#374051;">4.快速加工扫描的是成品，扫描</font><font style="color:#374051;">BOM</font><font style="color:#374051;">规则中的原料报错提示；</font>

<font style="color:#374051;">5.加工确认页面，修改成品商品数量，原料商品数量不再根据配比数增减；</font>

<font style="color:#374051;">6.加工确认页面，原料商品数量支持修改，修改单个原料的数量后不影响成品、其他原料的数量；</font>

<font style="color:#374051;">7.快速加工原料的库存扣减是在提交加工单时扣减；</font>

<font style="color:#374051;">8.PC上业务配置开启验货商品条码截取，</font><font style="color:#374051;">pda</font><font style="color:#374051;">会自动生效。若截取条码前</font><font style="color:#374051;">3</font><font style="color:#374051;">位，商品条码是</font><font style="color:#374051;">new0001</font><font style="color:#374051;">，则</font><font style="color:#374051;">pda</font><font style="color:#374051;">只需要扫描条码</font><font style="color:#374051;">new</font><font style="color:#374051;">即可。</font>                    

 



> 更新: 2026-05-14 11:04:32  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/cxhqadbmygsab6mq>