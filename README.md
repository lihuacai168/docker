# docker learning
sudo docker pull ubuntu:16.04 #拉去ubuntu，16.04版本image  
sudo docker images #列出所有的docker镜像  
sudo docker run -t -i ubuntu:16.04 /bin/bash #运行名字是ubuntu:16.04的image  
sudo docker run -it -d -p 233:2333 rikasai/wget-ssr:latest #运行REPOSITORY是rikasai/wget-ssr，tag是latest的images，并且把容器2333端口绑定到宿主机的233端口  
sudo docker ps #查看正在运行的docker container（容器）  
sudo docker ps -l #查看正在最近运行的docker container（容器）  
docker exec -i -t <CONTAINER_ID> bash #进入正在运行的container（容器）  
docker commit -m="change aria2 rpc secret " b81598020081 rikasai/ssr_caddy_filemanager_aria2 #更新镜像内容 -m是备注本次提交的内容，b81598020081是容器id
docker tag a4d196220797 rikasai/ubuntu-ssr:latest #给image添加repository和tag，a4d196220797是image id,rikasai是docker用户名，ubuntu-ssr是docker远程仓库的名字，latest是tag 
docker push rikasai/ubuntu-ssr:latest #推送到docker远程仓库，rikasai是docker用户名，ubuntu-ssr是docker远程仓库的名字，latest是tag









