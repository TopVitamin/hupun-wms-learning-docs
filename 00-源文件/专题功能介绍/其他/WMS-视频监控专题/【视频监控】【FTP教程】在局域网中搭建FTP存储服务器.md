# 【视频监控】【FTP教程】在局域网中搭建FTP存储服务器

### <font style="color:rgb(55, 64, 81);">1.防火墙配置</font>
<font style="color:rgb(55, 64, 81);">安装前，先将搭建服务器的电脑局域网内防火墙/杀毒软件关闭，或将软件设置为白名单（无杀毒软件可忽略）</font>

![1702344246135-99c6acd4-f862-4e23-b2bc-7609b6cecbda.png](./img/cTOa1t3L-7UqDsTP/1702344246135-99c6acd4-f862-4e23-b2bc-7609b6cecbda-347856.png)<font style="color:rgb(55, 64, 81);">  
</font>

### <font style="color:rgb(55, 64, 81);">2.服务器固定IP配置</font>
<font style="color:rgb(55, 64, 81);">在安装服务器的电脑上配置局域网固定IP</font>

+ <font style="color:rgb(55, 64, 81);">方法1:局域网路由器固定IP分配，设置方式</font>[参照链接(Tp-link)](https://resource.tp-link.com.cn/pc/docCenter/showDoc?id=1655112511768617)
+ <font style="color:rgb(55, 64, 81);">方法2:服务器电脑获取，设置方式</font>[参照链接](https://jingyan.baidu.com/article/f96699bbce85adc84f3c1b15.html)

### <font style="color:rgb(55, 64, 81);">3.下载服务器搭建工具FileZillaServer</font>
<font style="color:rgb(55, 64, 81);">打开网址，点击下载并安装，默认安装即可(目前最新版本为1.6.1）。</font>[下载地址](https://filezilla-project.org/download.php?type=server)

![1702344269395-2b65f5f9-8387-413e-b17e-9aaa85b49eed.png](./img/cTOa1t3L-7UqDsTP/1702344269395-2b65f5f9-8387-413e-b17e-9aaa85b49eed-316764.png)

![1702344294067-460ab02e-5474-4b54-94f5-eaa0755faaeb.png](./img/cTOa1t3L-7UqDsTP/1702344294067-460ab02e-5474-4b54-94f5-eaa0755faaeb-029675.png)![1702344303643-5e8b3778-37d6-4210-a4e7-9e128ae8559f.png](./img/cTOa1t3L-7UqDsTP/1702344303643-5e8b3778-37d6-4210-a4e7-9e128ae8559f-379647.png)![1702344324771-e176ad77-0e9a-407e-a40e-471c817f468d.png](./img/cTOa1t3L-7UqDsTP/1702344324771-e176ad77-0e9a-407e-a40e-471c817f468d-903388.png)![1702344342328-e484552f-2635-4c55-b950-55af690e38ac.png](./img/cTOa1t3L-7UqDsTP/1702344342328-e484552f-2635-4c55-b950-55af690e38ac-713125.png)![1702344246818-c1efd2b4-ae32-406f-8999-1d49a0e10fe3.png](./img/cTOa1t3L-7UqDsTP/1702344246818-c1efd2b4-ae32-406f-8999-1d49a0e10fe3-408807.png)

### <font style="color:rgb(55, 64, 81);">4.登陆FTPServer </font>
<font style="color:rgb(55, 64, 81);">点击连接，默认安装即可。界面默认登陆IP、端口号、密码（该部分与安装最后一步填写的端口号和密码一致），点击ok登陆成功</font>

![1702344246836-328ad688-70ee-4c10-b794-ab170f47a317.png](./img/cTOa1t3L-7UqDsTP/1702344246836-328ad688-70ee-4c10-b794-ab170f47a317-071757.png)

![1702344246875-ea49dc37-f594-413e-b387-c73234c4887c.png](./img/cTOa1t3L-7UqDsTP/1702344246875-ea49dc37-f594-413e-b387-c73234c4887c-933042.png)

### <font style="color:rgb(55, 64, 81);">5.为服务器添加用户/存储</font>
<font style="color:rgb(55, 64, 81);">1）连接服务器后，点击“Server->configure”，在FTPServer下点击“Add”，在Address下新增本机ip地址，</font>**<font style="color:rgb(55, 64, 81);">默认Port为21</font>**<font style="color:rgb(55, 64, 81);">，再次点击“Apply”</font>

![1702344374730-953c7384-2b29-4fa0-83f1-1e0374d68878.png](./img/cTOa1t3L-7UqDsTP/1702344374730-953c7384-2b29-4fa0-83f1-1e0374d68878-758678.png)

<font style="color:rgb(55, 64, 81);">2）点击“Server->configure”，在Users下点击“Add”新增用户名称和本机保存地址，设置“Native Path”为服务器录像保存位置；勾选使用该用户且支持新增该用户登陆密码</font>

![1702344383539-6ab3d3ad-a407-4799-be06-fd2a095fb2af.png](./img/cTOa1t3L-7UqDsTP/1702344383539-6ab3d3ad-a407-4799-be06-fd2a095fb2af-583046.png)

### <font style="color:rgb(55, 64, 81);">6.服务器访问测试</font>
<font style="color:rgb(55, 64, 81);">在局域网其他电脑上，文件资源管理器中输入ftp://192.168.60.61(第2步配置的局域网IP)及账号密码可测试是否连接上，连接上可查看ftp服务器上存储文件。</font>

![1702344393302-18143a8e-ac5f-4bac-a317-f6a54ce93695.png](./img/cTOa1t3L-7UqDsTP/1702344393302-18143a8e-ac5f-4bac-a317-f6a54ce93695-761600.png)



> 更新: 2023-12-21 18:33:28  
> 原文: <https://hupun.yuque.com/unzko7/lsbfg0/gpbau5948uuw9mcd>