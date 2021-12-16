5 cd 进入share目录，然后 用括号里指令(docker build -t longdb-vue:V1.0.0 . )构建镜像。（注意最后的 . ）


6:运行生成成功的镜像：docker run -p 3000:80 -d --name longdbvuejs 34d9e8770f1b

参数讲解：

run: 创建一个新的容器并运行一个命令
-d: 后台运行容器，并返回容器ID
-p: 端口映射，格式为：主机(宿主)端口:容器端口
--name="longdbvuejs": 为容器指定一个名称

34d9e8770f1b  --为生成好的images_id.

7:docker ps 指令查看有哪些在运行，上图中看到longvuejs在运行。（测试 http://193.112.82.83:3000/#/page2）