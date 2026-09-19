# PDA-播种验货

<font style="color:#374051;">播种验货，可以帮助用户使用料框模式盲扫商品来验货，当扫到的商品匹配上订单后，会显示对应的筐号，用户只需要将商品放入对应的播种框中，具体操作如下：</font>

<font style="color:#374051;">一、点击播种验货按钮，用户可见如图界面，扫描配货单号或者拣货筐编码进行验货。</font>

![1587980264912-5d72192e-a9ef-4a0b-a8c9-3f1fdc431a8b.jpeg](./img/qeRzUEd8ajlwxmIm/1587980264912-5d72192e-a9ef-4a0b-a8c9-3f1fdc431a8b-151762.jpeg)

<font style="color:#374051;">二、选择波次后，开启后置打印，扫描工作台编码。</font>

![1587980265077-b72a7580-32b6-49c5-8ce6-81701dbd1287.jpeg](./img/qeRzUEd8ajlwxmIm/1587980265077-b72a7580-32b6-49c5-8ce6-81701dbd1287-730706.jpeg)

<font style="color:#374051;">扫描波次中相应的商品条码，显示商品和对应的筐号。</font>

![1587980265236-b2cb80ed-d782-4cbd-bfa3-9c9e351b5f3d.jpeg](./img/qeRzUEd8ajlwxmIm/1587980265236-b2cb80ed-d782-4cbd-bfa3-9c9e351b5f3d-456122.jpeg)

<font style="color:#374051;">1.pc</font><font style="color:#374051;">上流程配置开启验货商品条码截取，</font><font style="color:#374051;">pda</font><font style="color:#374051;">会自动生效。若截取条码前</font><font style="color:#374051;">3</font><font style="color:#374051;">位，商品条码是</font><font style="color:#374051;">new0001</font><font style="color:#374051;">，则</font><font style="color:#374051;">pda</font><font style="color:#374051;">只需要扫描条码</font><font style="color:#374051;">new</font><font style="color:#374051;">即可完成验货。</font>

<font style="color:#374051;">2.pc</font><font style="color:#374051;">上流程配置开启商品序列号管理</font><font style="color:#374051;">-</font><font style="color:#374051;">选择序列号出库登记环节为验货，</font><font style="color:#374051;">pda</font><font style="color:#374051;">会自动生效。扫描开启序列号的商品条码时要输入正确的序列号才可以完成验货。</font>

<font style="color:#374051;">当未开始验货或者部分验货时，点击提交，查看到播种筐验货情况</font>

![1587980265488-e2693232-5e2d-43a2-84f8-f688b8cfe592.jpeg](./img/qeRzUEd8ajlwxmIm/1587980265488-e2693232-5e2d-43a2-84f8-f688b8cfe592-269566.jpeg)

1.  <font style="color:#374051;">播种筐中的“</font><font style="color:#374051;">X</font><font style="color:#374051;">”，表示该订单被拦截或者挂起。</font>

2.<font style="color:#374051;">已完成验货的绿色高亮显示。</font>

                        

<font style="color:#374051;">三、验货完成，点击提交，即可提交到下一环节且打印快递单。</font>

<font style="color:#374051;">1.</font><font style="color:#374051;">打印快递单时，</font><font style="color:#374051;">pc</font><font style="color:#374051;">和</font><font style="color:#374051;">pda</font><font style="color:#374051;">需处于同一局域网下且快递单模板时菜鸟模板。</font>

<font style="color:#374051;">2.</font><font style="color:#374051;">部分提交时，只打印已验货完成的订单。</font>

<font style="color:#374051;">3.</font><font style="color:#374051;">订单全部被拦截或挂起，不打印快递单。</font>

 



> 更新: 2023-12-21 09:28:17  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/wil6bzwnagbvnmwi>