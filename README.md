# flink_LogAnalysis
A log analysis program based on flink



## 项目介绍

该项目基于kafka和flink构建了一套实时日志分析系统。主要实现了热门商品统计、热门访问页面统计、PageView统计和UniqueVisitor统计四个需求。

HotItemsAnalysis模块实现了对事件时间升序排列后的日志，统计热门商品。

NetworkFlowAnalysis模块实现了对HotPages、PV、UV的统计处理。



## 项目运行环境



| requirements | version |
| ------------ | ------- |
| flink        | 1.10.1  |
| java         | 1.8     |
| kafka        | 3.0.0   |
| zookeeper    | 3.5.7   |



* 本项目基于三台ubuntu20.04虚拟机搭建的集群，用户可以根据自己的集群地址，手动调整kafka集群生产者和消费者地址。
* 可以根据集群版本，在主POM文件中修改对应版本。
