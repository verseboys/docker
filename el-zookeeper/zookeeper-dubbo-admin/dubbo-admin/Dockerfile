FROM openjdk:8

MAINTAINER 作者 <邮箱> #可选

# 注意 如果选择方式1编译dubbo-admin,此处 EVN 设置注册中心地址，方式2不需要在此处设置注册中心地址
#ENV DUBBO_IP_TO_REGISTRY zookeeper    服务名称/IP地址
#ENV DUBBO_PORT_TO_REGISTRY 12345       端口（默认不需要修改端口）

VOLUME /tmp

add dubbo-admin-0.0.1-SNAPSHOT.jar app.jar

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]