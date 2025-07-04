# Web集成靶场



#### 介绍
一个一键部署Web集成靶场在Centos7.6上的脚本，涵盖了如下5个Web常用靶场
1.  **upload-labs**
2.  **xss-labs**
3.  **sqli-labs**
4.  **pikachu**
5.  **dvwa**



#### 脚本搭建的安装（较慢）
1.  使用**image**目录下的镜像**CentOS-7-x86_64-DVD-1810.iso**在VM中新建一台虚拟机
2.  配置虚拟机的网络适配器为**NET**
3.  配置虚拟机的IP地址
4.  将**SRC**目录下的所有内容放在**/root/**目录下
5.  执行安装命令：**sed -i 's/\r$//' install.sh && chmod 777 install.sh && ./install.sh**
6.  等待安装成功后根据输出内容进入相应网址进行练习
![](https://gitee.com/APingu/picture/raw/master/20250704133637012.png)



#### 直接导入虚拟机的安装（快）
1.  **ova**目录下的**Web集成靶场.ova**下载下来直接导入虚拟机
2.  配置虚拟机的网络适配器为NET
3.  配置虚拟机的IP地址（虚拟机默认用户：**root**，密码：**password**）
4.  开机后访问配置好的IP地址即可进入管理页面



#### 默认配置的端口
1.  Web 集成靶场管理平台：**52000 OR 直接访问IP**

![Web 集成靶场管理平台](https://gitee.com/APingu/picture/raw/master/20250704133427999.png)

2.  upload-labs：**52001**

![upload-labs](https://gitee.com/APingu/picture/raw/master/20250704133444967.png)

3.  xss-labs：**52002**

![xss-labs](https://gitee.com/APingu/picture/raw/master/20250704133528932.png)

4.  sqli-labs：**52003**

![sqli-labs](https://gitee.com/APingu/picture/raw/master/20250704133536993.png)

5.  pikachu：**52004**

![pikachu](https://gitee.com/APingu/picture/raw/master/20250704133547672.png)

6.  web-dvwa：**52005**

![dvwa](https://gitee.com/APingu/picture/raw/master/20250704133556148.png)



#### 其他
1.  五个服务均设置了开机自启
2.  **dvwa**的初始用户：**admin**，密码：**password**