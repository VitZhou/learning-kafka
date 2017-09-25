# 介绍
### 为何说Kafka是一个分布式传输平台?
一般来说流媒体平台具备一下三个功能:
- 可以发布和订阅records streams,在这方面，它类似于消息队列或企业消息系统。
- 可以以容错方式存储records streams.
- 可以在records streams发生时进行处理。

### 它用于两大类应用程序：
- 构建可靠地在系统或应用程序之间获取数据的实时stream数据流水线
- 构建对数据流进行转换或响应的实时流应用程序

要了解Kafka如何做这些事情，让我们从下而上地研究和探索Kafka的功能。

### 概念
- Kafka作为群集可以在一个或多个服务器上运行。
- Kafka集群以称为topics(主题?)的categories存储records streams
- 每个record由一个键，一个值和一个时间戳组成

### Kafka有四个核心API：
- Producer API允许应用程序将记录流发布到一个或多个Kafka主题
- Consumer API允许应用程序订阅一个或多个主题(topics)，并处理为其生成的记录流(records streams)
- Streams API允许应用程序充当流处理器，消耗来自一个或多个主题(topics)的输入流并产生到一个或多个输出主题(topics)的输出流，有效地将输入流转换为输出流。
- Connector API允许构建和运行可重用的生产者或消费者，将Kafka主题连接到现有应用程序或数据系统。 例如，关系数据库的连接器可能捕获对表的每个更改。
