这是一个简单的spring cloud注册中心demo，使用eureka框架

application.yml中的配置：
1、阻止服务将自己作为客户端注册register-with-eureka:false 	fetch-registry:false
2、配置服务的域名：eureka.instance.hostname:localhost
3、配置默认的zone：eureka.client.service-url.defaultZone:http://${eureka.instance.hostname}:{server.port}/eureka,defaultZone只能这么写