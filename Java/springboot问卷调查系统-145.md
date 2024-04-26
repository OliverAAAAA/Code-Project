- 大家可以去[【公众号】](#联系我)获取或者加我[【微信】](#联系我)提意见(别忘记**Star**哟)。

<br/>
<div align="center">
    <a href="#联系我" style="text-decoration:none"><img src="../img/0d2eebe901258c45b2e7d06112d7026.png"></a>
</div>
<br/>


<p align="center">
  <a href="#联系我"><img src="https://img.shields.io/badge/weChat-微信群-blue.svg" alt="微信群"></a>
  <a href="#联系我"><img src="https://img.shields.io/badge/%E5%85%AC%E4%BC%97%E5%8F%B7-宝藏秘密基地Plus-lightgrey.svg" alt="公众号"></a>
  <a href="https://juejin.cn/user/1204720476893848/posts" target="_blank" ><img src="https://img.shields.io/badge/juejin-掘金-blue.svg" alt="公众号"></a>
  <a href="https://blog.csdn.net/OliverAAAAAA" target="_blank" ><img src="https://img.shields.io/badge/csdn-CSDN-red.svg" alt="CSDN"></a>
</p>

# 基于springboot+vue的“在线问卷调查系统”实现与设计（源码+数据库+文档)

-   开发语言：Java
-   数据库：MySQL
-   技术：SpringBoot、vue
-   工具：IDEA/Ecilpse、Navicat、Maven




## 系统展示



### 管理系统-登录页
![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/aef98d01d59745df85b9f057fd92e239~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=2375826&e=png&b=313c3f)


### 管理系统-问卷管理

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/6c52486d446d4a4eb78a6b2962b074a8~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=55876&e=png&b=f6f8fa)







### 管理系统-用户管理页面


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/50dc652597754be8836f6fba4b503b33~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=114191&e=png&b=f6f8fa)




### 管理系统-题目管理页面

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/f81054735560435dbeb906ba77a46c1a~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=98000&e=png&b=ffffff)

### 管理系统-问卷调查记录页面


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/39e35c2c9abc4bdbb646a66e658355f4~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=116769&e=png&b=ffffff)




### 管理系统-新闻资讯页面


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/48e6dd1d609d4ce7a54fa21a0f6e26cc~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=92765&e=png&b=f5f7fa)




### 管理系统-新闻类型页面

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/e63fc2acca7f455abb0f5817ef09e632~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=56404&e=png&b=f6f8fa)




### 管理系统-轮播图管理页面

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/bfd43816d1794ef685aa20dd6e4d9720~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=98982&e=png&b=fffefe)







### 前台-问卷列表

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/0fd3526ab22347599218e3372f8c568e~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=426705&e=png&b=fbf8f7)




### 前台-新闻资讯展示

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/c14e8b446b614a8e9a3fbf7408d66602~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=366833&e=png&b=fcfaf9)




### 前台-个人中心展示


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/62822c1315ae410db94fd30f5cc3c9e2~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=82560&e=png&b=ffffff)



## 摘要



  

如今社会上各行各业，都在用属于自己专用的软件来进行工作，互联网发展到这个时候，人们已经发现离不开了互联网。互联网的发展，离不开一些新的技术，而新技术的产生往往是为了解决现有问题而产生的。针对于问卷调查信息管理方面的不规范，容错率低，管理人员处理数据费工费时，采用新开发的在线问卷调查系统可以从根源上规范整个数据处理流程的正规性和合法性。

在线问卷调查系统能够实现问卷管理，用户管理，题目管理，问卷调查管理，新闻资讯管理等功能。该系统采用了Mysql数据库，Java语言，Spring Boot框架等技术进行编程实现。

在线问卷调查系统可以提高问卷调查信息管理问题的解决效率，优化问卷调查信息处理流程，并且能够保证存储数据的安全，它是一个非常可靠，非常安全的应用程序。


## 研究背景





  

二十一世纪互联网的出现，改变了几千年以来人们的生活，不仅仅是生活物资的丰富，还有精神层次的丰富。时代进步的标志，就是让人们过上更好的生活。在互联网诞生之前，地域位置往往是人们思想上不可跨域的鸿沟，信息的传播速度极慢，信息处理的速度和要求还是通过人们骑马或者是信鸽传递，这些信息传递都是不可控制的，中间很有可能丢失，信息的传递水平决定了人们生活的水平。现如今，大家都在用互联网来实现自己的目的，从内部管理设置计算机管理，提高内部信息管理水平，从外部市场也可以用计算机获取相关数据进行处理，如今各行各业已经严重依赖于计算机了。

本课题研究和开发在线问卷调查系统，让安装在计算机上的该系统变成管理人员的小帮手，提高问卷调查信息处理速度，规范问卷调查信息处理流程，让管理人员的产出效益更高。



## 研究意义

  

传统处理数据，必须是一张张纸，然后处理完毕又是统计在一张张纸上面，不断的重复处理，最终有个结果给最高层作为参考，这个模式在互联网没有出现之前，是一种常见的事情，信息管理的效率提不上去，那就用人才，人多力量大，是一个以前人们的常识。计算机的诞生就是发现了人多力量大的不足，比如高端计算人才的培养已经跟不上使用了，所以人们研究出专门帮助人们计算的机器，就是计算机的前身，到了互联网时代，人们发现完全可以让程序供应商提供解决方案，自己挑选自己合适的方案来提高自己的产出比。于是市面上就出现了各种各样的依靠程序处理信息的解决方案。

本课题研发的在线问卷调查系统，就是提供问卷调查信息处理的解决方案，它可以短时间处理完信息，并且只需要使用者动动鼠标和键盘就能获取自己需要的信息，并且这些信息都有专门的存储设备，而且数据的备份和迁移都可以设定为无人值守，从人力角度和信息处理角度以及信息安全角度，在线问卷调查系统是完胜传统纸质操作的，所以在线问卷调查系统就是如此的值得信赖。




## 系统功能架构图







![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/7bfd68258ca4432686adca493ba55686~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=546&h=486&s=22147&e=png&b=fcfcfc)

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/779f0217899f47d290569e8cfb7193b0~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=533&h=493&s=15292&e=png&b=fefefe)



部分代码展示



```
​​​
```



## 总结


在线问卷调查系统制作期间，我也遇到过一些难题，在最开始的时候，我并不知道该系统具体要设计几个功能模块，以及数据表需要设计几张表，还有对于开发技术的深度理论学习还不充分等，值得庆幸的是，我在面临这些困难时，我能够通过网络或者通过学院提供的图书馆寻求解决办法。比如在不知道具体功能的情况下，我从网上下载了很多的与在线问卷调查系统相关的程序，分析了它们的功能之后，我再结合即将开发的在线问卷调查系统进行综合分析，选取了适合在线问卷调查系统的功能部分，再结合实际情况以及使用者的需求确定本系统功能。对于数据表的设计，我先是在图书馆借阅了一本数据库方面的书籍进行查看，然后查看相似系统对于数据表的结构设计等知识，然后在本系统功能确定的情况下，结合本系统设计了配套的数据表，对于难度最大的开发技术部分，我花费了很多的时间研究网络上的相似系统的功能模块上的代码，一般都是对基础数据的增加，更新，查询或修改方面的代码，然后把本系统能够运用的代码部分在简单更改后进行使用，在完成了一个功能模块以及又一个功能模块之后，又经过了简单的测试工作，最终呈现出一个完整的能够解决用户实际问题的在线问卷调查系统。该系统唯一不足的就是代码方面还有很多重复的部分，不够精简，还有用户操作本系统，对于用户的误操作行为，本系统还不能及时反馈，这也是一大缺点。

在线问卷调查系统完成了，其相应的配套文档也需要进行编写，该文档主要描述在线问卷调查系统是如何进行分析，设计以及实现的，让其他阅读本文档的人增加对该系统的了解，编写文档过程中，由于自己平时对于办公软件的操作不是很频繁，根据学院要求的文档排版格式进行编辑也花了很多时间，在不断学习排版技巧以及对本系统配套文档的反复修改之后，最终在学院规定的时间内进行了文档定稿。




# 联系我
![gzhQr.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/d84631f305904993962172503d0fcc66~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=2023&h=624&s=5049546&e=bmp&b=fefefe)



**点击上方卡片关注私信我，回复145-A获取源码、文档及部署服务！**

## Github & Gitee

- [Github传送门](https://github.com/OliverAAAAA/Code-Project)
- [Gitee传送门](https://gitee.com/GuaGuaPool/Code-Project)

