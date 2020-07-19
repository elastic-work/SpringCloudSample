# SpringCloudSample
+ 子模块名字:cloud_pay_8001
+ pom依赖
+ 创建application.yml
```server:
   	port: 8001   
   spring:
   	application:
   		name: cloud-payment-service
   	datasource:
       # 当前数据源操作类型
       type: com.alibaba.druid.pool.DruidDataSource
       # mysql驱动类
       driver-class-name: com.mysql.cj.jdbc.Driver
         url: jdbc:mysql://localhost:3306/db2019?useUnicode=true&characterEncoding=
               UTF-8&useSSL=false&serverTimezone=GMT%2B8								
       username: root
       password: 123456
       #扫描对应的mapper映射文件
   mybatis:			
       mapper-locations: classpath*:mapper/*.xml
      	type-aliases-package: com.eiletxie.springcloud.entities
