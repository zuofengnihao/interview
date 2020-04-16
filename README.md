# interview

### Mybatis

什么是mybatis  
ORM框架 持久化框架 java通过JDBC协议连接数据库  
问题: 1.JDBC没有使用连接池 2.sql语句写在java代码中  

mappers加载mapper文件有几种方式:  
4种,resource|url|class|package,优先级:package 
   
### NIO

#### OSI七层模型

物理层 数据链路层 网络层 传输层 会话层 表示层 应用层

#### TCP/IP概念层模型

链路层 网络层 传输层`TCP/IP UDP` 应用层`HTTP`  

#### linux内核IO模型

1. 阻塞IO(BIO)
2. 非阻塞IO(Non Blocking IO)
3. IO多路复用(jdk1.4 NIO)
4. 信号驱动
5. 异步IO(jdk 1.7 NIO2 AIO)

Reactor模式与Proactor模式

面试题:
1. NIO与BIO的区别  
答：BIO是一个链接一个线程 NIO是单线程轮询selector上的状态
2. BIO和NIO的场景选择  
答：并发量小、数据量大。或者客户端可以选择BIO
3. Redis中使用的那种IO模型?什么线程模型?
答：Redis使用多路复用IO模型，线程是单线程的，redis操作都为原子操作。

###JVM