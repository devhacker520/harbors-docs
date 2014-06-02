# 安装HARBORS

    npm install harbors
    
或从github下载整个项目，[传送门](http://github.com/devhacker520/harbors-0.4.x.git)

# HARBORS简介

## HARBORS核心：

1. Server - 创建监听对象
2. VHost - 主机对象，如果没有区分主机，domain项可以填写*
3. Router - 负责当前主机内的路由规则传递以及规则解析

一个正常请求进入流程后首先被Server对象捕获，解析url后传递给对应的VHost对象，VHost再根据自身的一系列规则处理完请求后传递给Router，Router负责寻找对应的处理程序以及响应结果。

针对定制化要求不高的站点，HARBORS提供了Config类，Config可以负责处理传入的配置，并且自动生成对应的各个对象依赖，简化站点的开发流程。

## HARBORS类列表

harbors.**Server**： 监听实例

harbors.**VHost**： 主机实例

harbors.**Router**: 生成nodejs动态Router

harbors.**AutoRouter**： 在Router的基础上增加自动返回静态文件

harbors.**Config**： 解析配置文件的类

harbors.**Cluster**： 多进程集群模块

harbors.**Sync**： 异步方法的整理模块

harbors.**Directory**： 文件夹操作的功能集合

harbors.**String**： 字符串操作的功能集合

harbors.**Session**： session类，会自动为每个主机生成一个session对象负责处理对应功能

harbors.**Request**： request功能集合

harbors.**Response**： response类，res的功能都在这个类中声明

# 一些简单的示例

站点代码示例：[传送门](http://github.com/devhacker520/harbors-website.git)

测试例：[传送门](http://github.com/devhacker520/harbors-test.git)