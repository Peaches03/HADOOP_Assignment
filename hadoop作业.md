1\. Hive数据仓库在Hadoop中的作用

Hive是建立在Hadoo之上的一种数据仓库基础构架，可以存储查询和分析存储在Hado中的大规模数据。它提供了一系列的工具，可以用来进行数据的提开在馆及加载(ETL )。Hive定义了简单的类SOL查询语言，称为HOQL.它允许熟悉 so药化户查询数据。同时，这个语言也允许熟悉MapReduce的开发者开发自定义的MpeaReduce,以处理内建的Mapper和Reduce无法完成的复杂的分析工作。

Hive没有专门的数据格式，可以很好地工作在Thrift之上，控制分隔符，也允许用户指定数据格式。

作为Hadoop的数据仓库处理工具，Hive所有的数据都存储在Hadoop兼容的文件系统中。Hive在加载数据过程中不会对数据进行任何的修改，只是将数据移动到HDFS中Hive设定的目录下，因此，Hive 不支持对数据的改写和添加，所有的数据都是在加载的时候确定的。

1.  简述Hive清洗数据清洗的特点

    1.收集数据到Hadoop hdfs

    2.使用ETL(MapReduce)进行数据清洗

    3.更新元数据 target

    4.Hive 关联外部表

    5.创建工程

2.  Hive元数据库是用来干什么的，主要存储什么信息

    元数据：本质上只是用来存储hive中有哪些数据库，哪些表，表的模式，目录，分区，索引以及命名空间。为数据库创建的目录一般在hive数据仓库目录下。

    可以将原数据保存在关系数据库中，减少了在查询中执行语义的检查时间。
