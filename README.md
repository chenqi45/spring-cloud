# spring-cloud
此项目是springCloud的基础项目:
eureka-server : 服务注册中心 
hello-service : 服务提供方1
hello-service2 : 服务提供方2
eureka-ribbon : 负载均衡的消费者
启动步骤：
依次启动eureka-server、hello-service、hello-service2，启动后访问http://localhost:8010，
可以看到定义的服务被注册了hello-service：8021、hello-service2:8022
再启动消费者eureka-ribbon，访问http://localhost:8030/hello 两次，可以看到服务分别被访问一次
