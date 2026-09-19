# PDA-扫描打单

<font style="color:#374051;">业务场景：仓库操作员使用PDA领取波次任务，并直接打印电子面单，结合批量拣货、播种拣货，提升整体配货效率。 </font>

### <font style="color:#374051;">01.</font><font style="color:#374051;">领单配置</font>
<font style="color:#374051;">设置工作台，</font><font style="color:#374051;">PC</font><font style="color:#374051;">端设备管理，设置工作台的绑定库区、指定承运商、指定波次、绑定地址、打印机。</font>                  

![1587981706305-f6056b01-210b-4062-938a-8fbf66496bff.jpeg](./img/4Icg7fmZ-7EIfWIe/1587981706305-f6056b01-210b-4062-938a-8fbf66496bff-031321.jpeg)

<font style="color:#374051;">①、绑定库区：领单时，仅领取绑定库区的波次。</font>

<font style="color:#374051;">②、绑定地址：点击刷新，自动获取本机</font><font style="color:#374051;">ip</font><font style="color:#374051;">。③、指定承运商：领单时，仅领取指定承运商的波次；</font>

9.                        

<font style="color:#374051;">④、指定波次：领单时，仅领取指定的波次策略。</font>

<font style="color:#374051;">⑤、打印机设置：设置打印快递单的打印机。</font>

<font style="color:#374051;">检查网络，保证</font><font style="color:#374051;">PC</font><font style="color:#374051;">和</font><font style="color:#374051;">PDA</font><font style="color:#374051;">要在同一局域网，可以用</font><font style="color:#374051;">PDA</font><font style="color:#374051;">上的小工具检测，若是菜鸟控件运行正常，则</font><font style="color:#374051;">PC</font><font style="color:#374051;">和</font><font style="color:#374051;">PDA</font><font style="color:#374051;">在同一个局域网；若是报错，则检查</font><font style="color:#374051;">PC</font><font style="color:#374051;">和</font><font style="color:#374051;">PDA</font><font style="color:#374051;">网络。</font>                   

![1598425858281-9d3fac59-9cd6-4827-ba10-1615ef74e168.png](./img/4Icg7fmZ-7EIfWIe/1598425858281-9d3fac59-9cd6-4827-ba10-1615ef74e168-666597.png)

![1598425828708-ba3145b8-c29e-4e7e-a62c-1ab9e0e99b85.png](./img/4Icg7fmZ-7EIfWIe/1598425828708-ba3145b8-c29e-4e7e-a62c-1ab9e0e99b85-772022.png)

                    

<font style="color:#374051;">波次策略设置，指定的波次策略要开启允许</font><font style="color:#374051;">PDA</font><font style="color:#374051;">领单才能被领取到。</font>                  

![1587981707029-32ead7bb-5036-415b-9b15-af6de9ddfb13.jpeg](./img/4Icg7fmZ-7EIfWIe/1587981707029-32ead7bb-5036-415b-9b15-af6de9ddfb13-100756.jpeg)            

### <font style="color:#374051;">02.</font><font style="color:#374051;">扫描打单</font>
<font style="color:#374051;">具体步骤如下：</font>

1<font style="color:#374051;">点击扫描打单按钮，用户可见如图界面，输入工作台编码或扫工作台编码，领取任务。</font>                    

![1587981707220-bf695623-3ad3-402a-a62d-45b876a8a246.jpeg](./img/4Icg7fmZ-7EIfWIe/1587981707220-bf695623-3ad3-402a-a62d-45b876a8a246-306066.jpeg)

<font style="color:#374051;">2.</font><font style="color:#374051;">领取任务后，打印快递单，跳转到如图界面，用户选择拣货方式，进行拣货。</font>

![1587981707397-f711940f-5d26-4aa4-8d7b-46b6561c4f4d.jpeg](./img/4Icg7fmZ-7EIfWIe/1587981707397-f711940f-5d26-4aa4-8d7b-46b6561c4f4d-291556.jpeg)

![1587981707589-ce2dbc5a-87e6-47a8-8f75-ff786df803e7.jpeg](./img/4Icg7fmZ-7EIfWIe/1587981707589-ce2dbc5a-87e6-47a8-8f75-ff786df803e7-038158.jpeg)

<font style="color:#374051;">3.</font><font style="color:#374051;">拣货提交后，任务完成，即可再次扫工作台编码，领取下个任务。</font>

### <font style="color:#374051;">03.</font><font style="color:#374051;">领单逻辑</font>
1. <font style="color:#374051;">波次策略勾选了开启</font><font style="color:#374051;">PDA</font><font style="color:#374051;">允许领单</font><font style="color:#374051;">-</font><font style="color:#374051;">扫描打单，才能被领取到。</font>

2. <font style="color:#374051;">波次是待打单状态，才能被领取到。</font>

<font style="color:#374051;">3.波次中的订单都生成了电子面单，才能被领取到。</font>

<font style="color:#374051;">4.没有打印过快递单、发货单、配货单、发票的波次，才能被领取到。</font>

<font style="color:#374051;">5.与工作台设置的绑定库区、指定波次一致的波次，才能被领取到。</font>

<font style="color:#374051;">6.与工作台设置的指定承运商一致的波次，才能被领取到。</font>

<font style="color:#374051;">7.序列号登记环节在拣货且波次中含有序列号商品，该波次不能被领到。</font>

<font style="color:#374051;">符合条件的任务如何分配：</font>

<font style="color:#374051;">按当前正在拣货的库区</font><font style="color:#374051;">(</font><font style="color:#374051;">待拣货正在执行的波次任务</font><font style="color:#374051;">)</font><font style="color:#374051;">，库区中拣选人员最少的波次优先领取，如果跨区跟单区数量相同则跨区优先，越早生成的波次优先领取。</font>

<font style="color:#374051;">Ps.</font><font style="color:#374051;">目的是边拣边播动态分流，防止某个区人太多全部扎堆的交通堵塞，造成效率降低。</font>

 



> 更新: 2023-12-21 09:28:17  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/gg2t4fdo0erthxz1>