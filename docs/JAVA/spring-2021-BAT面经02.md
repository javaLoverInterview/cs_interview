1、SpringBoot运行项目的几种方式？
打包用命令或者放到容器中运行
1、 打成jar包，使用java -jar xxx.jar运行
2、 打成war包，放到tomcat里面运行
直接用maven插件运行 maven spring-boot：run
直接执行main方法运行


2、IOC的优点是什么？
IOC 或 依赖注入把应用的代码量降到最低。它使应用容易测试，单元测试不再需要单例和JNDI查找机制。最小的代价和最小的侵入性使松散耦合得以实现。IOC容器支持加载服务时的饿汉式初始化和懒加载。


3、在Spring MVC应用程序中使用WebMvcTest注释有什么用处？
WebMvcTest注释用于单元测试Spring MVC应用程序。我们只想启动ToTestController。执行此单元测试时，不会启动所有其他控制器和映射。
@WebMvcTest(value = ToTestController.class, secure = false):
4、什么是Spring Cloud？
根据Spring Cloud的官方网站，Spring Cloud为开发人员提供了快速构建分布式系统中一些常见模式的工具（例如配置管理，服务发现，断路器，智能路由，领导选举，分布式会话，集群状态）。
5、eureka服务注册与发现原理
1、 每30s发送⼼跳检测重新进⾏租约，如果客户端不能多次更新租约，它将在90s内从服务器注册中⼼移除。
2、 注册信息和更新会被复制到其他Eureka 节点，来⾃任何区域的客户端可以查找到注册中⼼信息，每30s发⽣⼀次复制来定位他们的服务，并进⾏远程调⽤。
3、 客户端还可以缓存⼀些服务实例信息，所以即使Eureka全挂掉，客户端也是可以定位到服务地址的。

6、SpringBoot 配置文件的加载顺序
由jar包外向jar包内进行寻找;
优先加载带profile
jar包外部的application-{profile}.properties或application.yml(带spring.profile配置文件
jar包内部的application-{profile}.properties或application.yml(带spring.profile配置文件
再来加载不带profile
jar包外部的application.properties或application.yml(不带spring.profile配置文件
jar包内部的application.properties或application.yml(不带spring.profile配置文件
7、什么是 spring 装配
当 bean 在 Spring 容器中组合在一起时，它被称为装配或 bean 装配。Spring 容器需要知道需要什么 bean 以及容器应该如何使用依赖注入来将 bean 绑定在一起，同时装配 bean。
8、为什么要用SpringBoot
快速开发，快速整合，配置简化、内嵌服务容器
9、怎么样把ModelMap里面的数据放入Session里面？
可以在类上面加上@SessionAttributes注解,里面包含的字符串就是要放入session里面的key。
10、什么是微服务架构中的DRY？
DRY代表不要重复自己。它基本上促进了重用代码的概念。这导致开发和共享库，这反过来导致紧密耦合。
11、使用Spring Cloud有什么优势？
12、负载平衡的意义什么？
13、SpringBoot 中的 starter 到底是什么 ?
14、Spring对DAO的支持
15、介绍一下 WebApplicationContext
16、什么是 Spring Framework？
17、为什么要使用 Spring Cloud 熔断器？
18、Spring Cloud的版本关系
19、SpringBoot、Spring MVC 和 Spring 有什么区别
20、DiscoveryClient的作用
21、什么是嵌入式服务器？我们为什么要使用嵌入式服务器呢?
22、什么是Spring的内部bean？
23、SpringBoot 的核心配置文件有哪几个？它们的区别是什么？
24、网关与过滤器有什么区别
25、描述一下 DispatcherServlet 的工作流程
26、SpringBoot集成mybatis的过程
27、什么是 Aspect 切面
28、Spring Cloud Gateway
29、Zuul网关如何搭建集群
30、什么是 JavaConfig？
31、使用 SpringBoot 启动连接到内存数据库 H2 的 JPA 应用程序需要哪些依赖项？