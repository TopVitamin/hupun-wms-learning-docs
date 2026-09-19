# PDA-自由领单

<font style="color:#374051;">业务场景：针对一种一件的订单，特别是服装相关行业（订单比例可大于60-70%），希望有比目前系统更加相对便捷简单的拣货。</font>

### <font style="color:#374051;">01.</font><font style="color:#374051;">自由领单</font>
<font style="color:#374051;">具体步骤如下：</font>

<font style="color:#374051;">1.</font><font style="color:#374051;">点击自由领单按钮，用户可见如图界面，选择作业库区，点击领取任务按钮，操作员领取到任务并进行作业。</font>

![1588056238745-f19bd50d-0de1-4d82-8db5-9f5ba0240368.jpeg](./img/v149Cv-wNr6HCv1M/1588056238745-f19bd50d-0de1-4d82-8db5-9f5ba0240368-793119.jpeg)

<font style="color:#374051;">2.</font><font style="color:#374051;">领取任务后，跳转到如图界面，操作员进行拣货。</font>

![1588056238937-ae600b92-6111-468c-86e5-a0aa70ff0e7e.jpeg](./img/v149Cv-wNr6HCv1M/1588056238937-ae600b92-6111-468c-86e5-a0aa70ff0e7e-353889.jpeg)

<font style="color:#374051;">3.</font><font style="color:#374051;">拣货提交后，任务完成，即可点击领取任务，领取下个任务。</font>

### <font style="color:#374051;">02.</font><font style="color:#374051;">领单逻辑</font>
<font style="color:#374051;">1.</font><font style="color:#374051;">正常领取情况，前提都是自由波次</font>

<font style="color:#374051;">①</font><font style="color:#374051;">.</font><font style="color:#374051;">若操作员已有拣货任务，进入自由领单菜单后自动加载该任务。</font>

<font style="color:#374051;">②</font><font style="color:#374051;">.</font><font style="color:#374051;">波次中有部分订单被拦截或挂起，该波次可以被正常领取。</font>

<font style="color:#374051;">③列号登记环节在验货环节，波次中的订单有序列号商品，该波次可以被正常领取。</font>

<font style="color:#374051;">④</font><font style="color:#374051;">.</font><font style="color:#374051;">波次上无打印标记，订单有或没有打印标记，该波次可以被正常领取。</font>

<font style="color:#374051;">⑤.波次中的订单都生成电子面单，该波次可以被正常领取</font>（后台开关可配置领取无电子面单波次）<font style="color:#374051;">。</font>

<font style="color:#374051;">⑥</font><font style="color:#374051;">.</font><font style="color:#374051;">自由波次生成波次后，策略停掉，该波次可以被正常领取。</font>

<font style="color:#374051;">2.</font><font style="color:#374051;">领取不到情况</font>

<font style="color:#374051;">①</font><font style="color:#374051;">.</font><font style="color:#374051;">所选作业库区下无自由波次，领取不到任务。</font>

<font style="color:#374051;">②</font><font style="color:#374051;">.</font><font style="color:#374051;">波次的拣选区域为空，领取不到任务。</font>

<font style="color:#374051;">③.波次上有打印标记，该波次不能被领取到。</font>

<font style="color:#374051;">④.序列号登记环节在打单或拣货环节，波次中的订单有序列号商品，该波次不能被领取到。</font>

<font style="color:#374051;">⑤.无拣货环节，不能领取到任务。</font>

<font style="color:#374051;">⑥.波次中的订单都被拦截或挂起，该波次不能被领取到。</font>

<font style="color:#374051;">⑦.领取不到符合扫描打单或料筐拣货的波次。</font>

<font style="color:#374051;">3.</font><font style="color:#374051;">领单顺序</font>

<font style="color:#374051;">优先标记的波次（订单中标记预售</font><font style="color:#374051;">></font><font style="color:#374051;">天猫直送</font><font style="color:#374051;">>COD</font><font style="color:#374051;">订单</font><font style="color:#374051;">></font><font style="color:#374051;">加急订单）</font><font style="color:#374051;">></font><font style="color:#374051;">区域库区下的作业数（少</font><font style="color:#374051;">></font><font style="color:#374051;">多）</font><font style="color:#374051;">></font><font style="color:#374051;">波次生成时间（早</font><font style="color:#374051;">></font><font style="color:#374051;">晚）</font><font style="color:#374051;">></font><font style="color:#374051;">波次优先级（高</font><font style="color:#374051;">></font><font style="color:#374051;">低）</font><font style="color:#374051;">></font><font style="color:#374051;">波次库区</font><font style="color:#374051;">ID</font><font style="color:#374051;">（小</font><font style="color:#374051;">></font><font style="color:#374051;">大）</font>

 



> 更新: 2024-10-15 11:15:41  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/lu9gz5wg7bc29wdu>