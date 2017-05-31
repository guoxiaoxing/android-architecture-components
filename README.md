# Android Architecture Components

**关于作者**

>郭孝星，非著名程序员，主要从事Android平台基础架构与中间件方面的工作，爱好广泛，技术栈主要涉及以下几个方面
>
>- Android/Linux
>- Java/Kotlin/JVM
>- Python
>- JavaScript/React/ReactNative
>- DataStructure/Algorithm
>
>文章首发于[Github](https://github.com/guoxiaoxing)，后续也会同步在[简书](http://www.jianshu.com/users/66a47e04215b/latest_articles)与
[CSDN](http://blog.csdn.net/allenwells)等博客平台上。文章中如果有什么问题，欢迎发邮件与我交流，邮件可发至guoxiaoxingse@163.com。

Android应用开发架构一直没有一套官方的标准，各公司在架构的选择上也有MVC、MVP与MVVM很多种，我们公司一直在使用的是MVP+Dagger的方式，个人感觉不是理想
的选择，一来代码臃肿，二者也不是很直观。良好的开发架构必然是既能做到良好的解耦，又能提升开发者的开发效率。

好在在今年的Google IO 2017大会上，Google不仅将Kotlin正式纳入官方开发语言，还提出了Android Architecture Components这一套框架。

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

这套框架强调以下两点：

```
1 不要在应用程序组件中保存应用数据，应用组件间也不应该互相依赖。
2 通过Model驱动UI，并做好数据持久化。
```

文章目录

**应用开发架构篇**

- [1应用开发架构篇：Activity与Fragment生命周期处理](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/应用开发架构篇/1应用开发架构篇：Activity与Fragment生命周期处理)
- [2应用开发架构篇：动态数据](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/应用开发架构篇/2应用开发架构篇：动态数据.md)
- [3应用开发架构篇：数据绑定](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/应用开发架构篇/3应用开发架构篇：数据绑定.md)
- [4应用开发架构篇：Room ORM框架](https://github.com/guoxiaoxing/android-architecture-components/blob/master/doc/应用开发架构篇/4应用开发架构篇：Room ORM框架.md)