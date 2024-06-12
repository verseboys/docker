生成镜像

docker build -t dubbo-admin:1.0 .


再执行
docker-compose up -d 

## 启动 ##
docker-compose up
#查看时候有异常抛出，检查配置中心地址指向是否正确，如果没有错误,结束服务
docker-compose up -d #后台运行
检查
http://IP:7001 登录 系统管理 系统状态 是否正常

账号 root 密码:root

作者：额嗬
链接：https://www.jianshu.com/p/5314cae6aaca
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
