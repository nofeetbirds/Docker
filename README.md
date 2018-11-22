# Docker

gitlab

docker 安装gogos 教程 https://www.jianshu.com/p/64e9708c23e7

拉取镜像：docker pull nginx
创建容器： docker run -d --name nginx nginx
部署命令： docker run -d -p 8081:80 --name nginx-web-6666 -v $PWD/html:/usr/share/nginx/html -v $PWD/conf/nginx.conf:/etc/nginx/nginx.conf -v $PWD/logs:/var/log/nginx nginx

路径必须存在不然就不可以运行

拷贝工程文件到docker中
docker cp /home/usr01/lwx/runing_pro/Testplatform    9e2xxxxx:/home/html    <---这里的容器id要全

进入容器内部
docker exec -it id /bin/bash 

