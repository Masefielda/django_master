#文档#
[最小物联网系统文档](https://github.com/gmszone/iot-doc)

#Minimum Internet of Things#
A Minimum IOT with arduino and raspberry pi.

一个最小的物联网系统设计方案及源码

    android/ 一个最小的Android程序实例
    rest/ PHP Laravel Framework to create RESTful API
    python/ 简单的pyhon示例
    hardware/  硬件串口通信收集
	 -/ arduino Arduino板
    doc/  文档 简介ppt nginx配置 系统框架图
    dashboard/ 基于ruby框架dashing的dashboard

##简要的初始化代码说明##
代码中因为有两个子模块，即Android与REST，Android是一个简单的Android程序示例,REST作为子模块的原因是考虑到后期会用更简单的源码来替换。但是laravel作为一个运行环境，还是很理想的。

先clone

    git clone https://github.com/gmszone/iot.git iot

子模块

    git submodule init
    git submodule update

##系统框架图##

![](https://raw.github.com/gmszone/iot/master/doc/dot/struct.jpg)

##如何在电脑上测试

 1. 有一个Arduino开发板.

 2.将arduino/BareMinimum.ino 烧录到开发板上


 3. 如果用的是Windows系统 需要将get.py中的 /dev/ttyACM0 改为 COM*.

        cd python
        sudo python get.py

 4. 打开 localhost/athome/create to 创建一个数据。打开 /athome/1/edit 编辑状态

 5. 作为测试，你可以访问[b.phodal.com][1]

##如何在Android手机上测试

![](https://raw.github.com/gmszone/iot/master/doc/images/android.png)

  1. 下载安装 [Stay at Home][13]

##中文文档

[一个最小的物联网系统设计方案及源码][2]

[最小物联网系统（一）——系统组成][4]

[最小物联网系统（二）——RESTful][5]

[最小物联网系统（三）——创建RESTful][6]

[最小物联网系统（四）——详解Laravel的RESTful][7]

[最小物联网系统（五）——Laravel RESTful模板化][8]

[最小物联网系统（六）——Ajax打造可视化][9]

[最小物联网系统（七）——与服务器通讯][10]

[最小物联网系统（八）——与单片机通讯][11]

[最小物联网系统（九）——Android客户端][12]

[最小物联网系统设计——给Laravel添加测试][15]

[最小物联网系统——Dashboard][16]

## Liscense

© 2014 Phodal Huang. This code is distributed under the MIT license.

[1]:http://b.phodal.com
[2]:http://www.phodal.com/blog/bare-minimum-iot
[3]:https://github.com/gmszone/iot/wiki
[4]:http://www.phodal.com/blog/bare-minimum-iot-system-structure/
[5]:http://www.phodal.com/blog/bare-minimum-iot-system-restful/
[6]:http://www.phodal.com/blog/bare-minimum-iot-system-create-restful/
[7]:http://www.phodal.com/blog/bare-minimum-iot-system-about-restful/
[8]:http://www.phodal.com/blog/bare-minimum-iot-system-restful-template/
[9]:http://www.phodal.com/blog/bare-minimum-iot-system-ajax/
[10]:http://www.phodal.com/blog/bare-minimum-iot-system-date-commucation/
[11]:http://www.phodal.com/blog/bare-minimum-iot-system-mcu-commucation/
[12]:http://www.phodal.com/blog/bare-minimum-iot-system-android-example/
[13]:https://github.com/gmszone/Home-Anywhere/raw/master/app/build/apk/app-debug-unaligned.apk
[14]:http://bbs.phodal.com
[15]:http://www.phodal.com/blog/bare-minimum-iot-system-add-test-for-laravel/
[16]:http://www.phodal.com/blog/bare-minimum-iot-system-dashboard-framework-dashing/
