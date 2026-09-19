# PDA-大宗拣货

<font style="color:#374051;">业务场景：订单是大宗件，商品种类和数量很多，可以把该订单拆分多个任务，分配给多人操作，也支持部分拣货，实现边拣货边装箱。</font>

1. <font style="color:#374051;">点击大宗拣货按钮，用户可见如图页面，扫描作业单号/系统单号/运单号或选择作业区域下拉选择任务。</font>                       

<font style="color:#374051;">  </font>![1593416987502-388d2a5d-ff8d-4f01-8e13-d6ba10bbdddc.png](./img/qIWG6Uy2t34WPOBg/1593416987502-388d2a5d-ff8d-4f01-8e13-d6ba10bbdddc-758235.png)

<font style="color:#374051;">注意：订单锁定成功未拆分，大宗拣货扫描系统单号/运单号，会直接生成一个拣货任务</font>

<font style="color:#374051;">2.页面下拉，加载作业区域下的任务所属订单，点击选择任务。</font>

<font style="color:#374051;">  </font>![1593417099614-df931702-6b36-45b2-8a1a-daee275c31bb.png](./img/qIWG6Uy2t34WPOBg/1593417099614-df931702-6b36-45b2-8a1a-daee275c31bb-831141.png)

<font style="color:#374051;">提示：</font>

<font style="color:#374051;">①、加载订单：作业区域下的任务所属订单且该订单下有任务时未完成的，全部任务完成的订单不加载、被拦截的订单不加载。</font>

<font style="color:#374051;">②、扫描任务单号时，不限制作业区域。</font>

<font style="color:#374051;">③、订单中任务排序显示：作业中无操作员</font><font style="color:#374051;">></font><font style="color:#374051;">未作业</font><font style="color:#374051;">></font><font style="color:#374051;">作业中有操作员</font><font style="color:#374051;">></font><font style="color:#374051;">已完成</font><font style="color:#374051;">.</font>

<font style="color:#374051;">3.选择任务，跳到拣货页面，进行拣货。</font>

<font style="color:#374051;">   </font>![1593417135962-cd0a1ccb-7277-46c9-990a-a89f36e49a44.png](./img/qIWG6Uy2t34WPOBg/1593417135962-cd0a1ccb-7277-46c9-990a-a89f36e49a44-495192.png)

<font style="color:#374051;">4.若仓库中的业务配置开启了大宗订单部分出库，部分拣货，点击提交，可以先提交已拣货的部分。</font>

![1593417177278-f95e72d9-d127-4740-8e49-8cc28ac901bd.png](./img/qIWG6Uy2t34WPOBg/1593417177278-f95e72d9-d127-4740-8e49-8cc28ac901bd-860052.png)

<font style="color:#374051;">提示：已拣的部分提交并拆出新的任务，状态是作业完成，提交后剩余未拣货的仍属于原任务且还是被当前操作员领取到。</font>

 



> 更新: 2024-02-06 09:34:02  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/dqsavnzc1gdgi0fe>