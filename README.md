# Android Architecture Components

作者: 郭孝星
邮箱: guoxiaoxingse@163.com
博客: http://blog.csdn.net/allenwells
简书: http://www.jianshu.com/users/66a47e04215b/latest_articles

**关于作者**

>郭孝星，非著名程序员，主要从事Android平台基础架构与中间件方面的工作。技术栈主要涉及Android/Linux, Java/Kotlin/JVM，Python, JavaScript/React/ReactNative，数据结构与算法等方面。热爱编程与吉他，喜欢有趣的事物和人。

**关于文章**

>作者的文章首发在[Github](https://github.com/guoxiaoxing)上，也会发在[简书](http://www.jianshu.com/users/66a47e04215b/latest_articles)与[CSDN](http://blog.csdn.net/allenwells)平台上，文章内容主要包含Android/Linux, Java/Kotlin/JVM，Python, JavaScript/React/ReactNative, 数据结构与算法等方面的内容。如果有什么问题，也欢迎发邮件与我交流。


在今年的Google IO 2017大会上，关于Android方面的内容的重磅新闻，除了Kotlin正式被纳入官方开发语言以外，就是
Android Architecture Components。

[Android Architecture Components官方文档](https://developer.android.com/topic/libraries/architecture/index.html)

>A new collection of libraries that help you design robust, testable, and maintainable apps. Start 
with classes for managing your UI component lifecycle and handling data persistence.


简单来说，就是一套基于数据持久化（Room ORM），Repository，ViewModel响应式渲染（LiveData）与Activity/Fragment生命周期处理的
整体框架。

所以你可以看到这套框架包含4个方面的内容：

- Handling lifecycles：创建一套UI可以自动响应生命周期的变化
- LiveData：当数据对象发生变化时可以自动通知UI
- ViewModel：存储UI所需相关数据
- Room：Google官方的ORM框架，比SQLite更加强大和安全

所以后续的文章会从这4个方面来介绍这套框架。

文章目录

- [1Android Architecture Components框架：Activity与Fragment生命周期处理](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/1Android Architecture Components框架：Activity与Fragment生命周期处理)
- [2Android Architecture Components框架：动态数据](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/2Android Architecture Components框架：动态数据.md)
- [3Android Architecture Components框架：数据绑定](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/3Android Architecture Components框架：数据绑定.md)
- [4Android Architecture Components框架：Room ORM框架](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/4Android Architecture Components框架：Room ORM框架.md)