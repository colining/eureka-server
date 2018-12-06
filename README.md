# Eureka功能
1. 服务的注册与发现，采用C-S的设计架构。各个服务都是客户端，都要到Eureka
这个服务器上注册
2. 改变了传统服务间的调用，链式调用被分割。
3. 作为轮询负载均衡器(算法为最简单的轮询)
4. 故障转移

# Eureka的基本架构
* Eureka，注册中心
* provider, 服务提供者，注册到Eureka上供别人调用
* consumer，服务的消费者

# 实践
1. pom引入相关包
2. 项目入口添加注解
3. properties中做相关配置，需要注意的一点事，注册中心会尝试注册自己，
要禁用这个行为

# 参考
[ityouknow](http://www.ityouknow.com/springcloud/2017/05/10/springcloud-eureka.html)