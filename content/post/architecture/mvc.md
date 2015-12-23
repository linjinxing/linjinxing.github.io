+++
banner = "banners/placeholder.png"
categories = ["软件架构"]
date = "2015-12-22T13:39:46+02:00"
tags = ["MVC","架构","耦合","重用","开发效率","扩展","设计模式","分层","T4"]
title = "MVC架构"
+++

 ## 本文试图解决以下问题：
- 掌握MVC架构
- 根据设计模式的单一职责，理清MVC中M,V,C的职责，特别是C(Controller)的职责，很多人对其有比较大的误解
- 做架构设计时，如何应用MVC做设计
- MVC架构中主要使用的设计模式

什么？还有没被满足的需求？请添加QQ群：515767434，我会尽力帮你解决。和MVVM，MVP的区别将在另一篇中介绍。


## 简介
MVC全名是Model View Controller，是模型(model)－视图(view)－控制器(controller)的缩写，一种软件设计典范，用一种业务逻辑、数据、界面显示分离的方法组织代码，将业务逻辑聚集到一个部件里面，在改进和个性化定制界面及用户交互的同时，不需要重新编写业务逻辑。[(百度百科解释)](http://baike.baidu.com/view/5432454.htm?fromtitle=mvc&fromid=85990&type=syn)

## 为什么使用MVC
* 耦合性低<br>
   视图层和业务模型层完全分离，它们之间没有任何耦合，因此视图层和业务层可以随意地变化，而这也符合设计模式的[迪米特原则](http://baike.baidu.com/view/823220.htm)。

* 重用性高<br>
  由于视图层和业务模型层完全分离，能很大程度上保证他们被[继承，组合，关联，依赖](http://blog.csdn.net/kevin_darkelf/article/details/11371353)。

* 容易分工，提高开发效率<br>
  可以将界面和模型层分配给两个人同时进行开发，缩短开发周期。

* 扩展容易<br>
  界面变化时，业务模型层可以完全保持不变，反之亦然。

## 定义
* Model（数据模型）<br>
模型封闭了业务逻辑和数据处理。模型的唯一职责：承担数据处理。

* View（视图）<br>
视图是用户可以看到的部分。视图的唯一职责：负责展示数据模型层传递的数据以及用户行为响应。

* Controller（控制器）<br>
控制器是一个或者多个M和一个或者多个V之间的中介，是M和V之间数据交换的桥梁。控制器职责：负责M和V之间的数据交换。

## 几种模式分析
- **传统MVC**
![传统MVC](../../../../images/traditional_mvc.gif)

传统模式V和M之间需要相互调用，知道对方的存在，明显耦合度比较高。

- **进化的MVC**
![进化的MVC](../../../../images/model_view_controller_2x.png)

当V层用户事件发生时，用户事件传递到C层，C层再调用M层响应用户事件，可能是从服务器获取数据，或者更新，删除数据。<br>
当M层数据变化时，会通知C层，C层再调用V层接口更新用户界面，完成更新操作。



## 架构分层

## 用到的设计模式简介
- 中介者
- 组合
- 职责链
- 策略
- 观察者

## MVC的缺点
- 


参与资料：

- [苹果开发官网：Model-View-Controller](https://developer.apple.com/library/ios/documentation/General/Conceptual/DevPedia-CocoaCore/MVC.html)




