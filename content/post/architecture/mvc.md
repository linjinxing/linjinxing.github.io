+++
banner = "banners/placeholder.png"
categories = ["软件架构"]
date = "2015-12-22T13:39:46+02:00"
tags = ["MVC","架构","耦合","重用","开发效率","扩展","设计模式","分层"]
title = "MVC架构"
+++

   MVC全名是Model View Controller，是模型(model)－视图(view)－控制器(controller)的缩写，一种软件设计典范，用一种业务逻辑、数据、界面显示分离的方法组织代码，将业务逻辑聚集到一个部件里面，在改进和个性化定制界面及用户交互的同时，不需要重新编写业务逻辑。[(百度百科解释)](http://baike.baidu.com/view/5432454.htm?fromtitle=mvc&fromid=85990&type=syn)

1. **为什么使用MVC**
   * 耦合性低
   
         视图层和业务模型层完全分离，它们之间没有任何耦合，因此视图层和业务层可以随意地变化，而这也符合设计模式的[迪米特原则](http://baike.baidu.com/view/823220.htm)。
   * 重用性高
     
         由于视图层和业务模型层完全分离，能很大程度上保证他们被[继承，组合，关联，依赖](http://blog.csdn.net/kevin_darkelf/article/details/11371353)。
   * 容易分工，提高开发效率
   
         可以将界面和模型层分配给两个人同时进行开发，缩短开发周期。
   * 扩展容易
   
         界面变化时，业务模型层可以完全保持不变，反之亦然。

2. **定义**
   * Model（数据模型）
    
        模型封闭了业务逻辑和数据处理。模型的唯一职责：承担数据处理。
   * View（视图）
   
        视图是用户可以看到的部分。视图的唯一职责：负责展示数据模型层传递的数据以及用户行为响应。
   * Controller（控制器）
   
        控制器是
3. **几种模式分析**
  
4. **架构分层**

5. **用到的设计模式简介**

参与资料：

[苹果开发官网：Model-View-Controller](https://developer.apple.com/library/ios/documentation/General/Conceptual/DevPedia-CocoaCore/MVC.html)




