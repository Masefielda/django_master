

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
