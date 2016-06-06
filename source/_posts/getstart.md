title: 写这一系列的目的
date: 2015-11-30 18:30:14
tags:
---
## java现状
Java难么，难，不难。模块就那么点东西，孰优孰劣根本就界限不太清晰，所以一般Java面试都会去拼广度，或者拼深度。可惜的是，就那么点有限的东西，工作个四五年的人竟有很大一部分概念模糊，实在让人不解。一来说明本行业严重缺人，滥竽充数一直可行；二来说明人心浮躁，java工厂化已经形成；更近一步说明，其实日常工作中，打交道的知识，其实都是烂大街的。
总结起来，有几个行业的知识面比较缺乏：

* 传统行业的Java程序员，做的都是些低访问量的管理系统，就是CRUD
* 做BI想转行的Java程序员，`BI`听起来高大上，其实用的东西就呵呵了
* 做数据挖掘搞大数据的，大多数拿别人架子搭平台，搞算法的才是正道
* 刚毕业，以为SSH就是全部的小鲜肉，那是几年前的事了
* 专搞业务的，您是领导，就不要来抢Java饭碗了

写这篇文章的另一个原因，是为了专业的有追求的程序员。你可能中间阶段经历了创业、或者其他原因比如转`Android`一段时间放弃了Java的、想去那些可恶的大公司但补充知识补差的，如果想回到Java开发的怀抱里来，这里会说明初中高级别的程序员所需要的知识素养。

繁忙的工作会占据你绝大多数时间，但，不要忘了学习。这个行业，不学习就等着被淘汰吧。

## 举个例子
java的内容其实也挺复杂的，举个例子：我经常问的一个问题就是：Java中`Object`类，都有哪些方法。看着挺简单的一道题目。但只此一题，便可分别三六九等。`Object`无非就这么几个方法，但考察的知识点就不一样了
``` java
getClass()
hashCode()
equals()
clone()
toString()
notify()
notifyAll()
wait()
finalize()
```

#### getClass

* 初级：classloader的加载顺序
* 中级：我可以加载一个网络上的class么，jar包呢
* 高级：OSGI的类加载机制是什么样的，tomcat呢

#### hashCode equals

* 初级：hashCode和equals是干什么用的
* 中级：HashMap的存储结构是什么，ConcurrentHashMap呢
* 高级：HashMap的Hash函数为什么要这么设计，HashTable呢

#### clone

* 初级：什么叫浅拷贝，什么叫深拷贝
* 中级：clone怎么做深拷贝，还有其他方式做深拷贝么
* 高级：为什么java已经有了clone方法，还要实现一个Cloneable接口呢

#### notify notifyAll wait

* 中级：wait和sleep有什么区别，应用场景，调用Thread的wait方法含义(陷阱)
* 高级：wait的参数，怎么判断wait是超时返回还是其他线程通知返回的呢？怎么查看处于wait状态的线程

#### finalize
* 中级：怎么阻止一个非根引用对象被回收
* 高级：一个空的Object占用多少内存，如果里面有空的`boolean`和`int`呢


本系列针对不同层次的人才，各分为`初级篇`，`中级篇`，`高级篇`，界限会有模糊，请自行斟酌，内容大体包括：

* `面向对象基本点`
* `集合操作`
* `多线程`
* `NIO/Netty`
* `网络`
* `JVM`
* `HTTP`
* `Linux`
* `DBMS(Mysql)`
* `NoSql(Redis)`
* `分布式`
* `中间件`
* `安全`
* `知识面测试`
* `其他杂乱的`

java这么多年的发展，枝叶繁杂，在这里，只谈基础。