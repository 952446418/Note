# docker

## 容器设置

### Py自动生成requirements.txt文件
pip freeze > requirements.txt
pipreqs --force ./ --encoding=utf-8

### 查询容器ID
docker ps

### 重命名
 docker rename 02（ID） myununtu

### 传文件进docker指定路径（容器）
dockerfile里写好
	COPY PointerNet_Chinese_Information_Extraction-main ./software/

### 看容器的ip地址
docker inspect ID
ping IP地址

### 传文件进docker指定路径（镜像）
docker cp /路径/文件名 容器ID:/上传路径

### 从docker传文件到实体机
docker cp 容器ID:/上传路径 /路径/文件名


### 运行进入
docker run -it ubuntu_py3:20.04
docker run -p 50051:50051 -it eventexsrv:0.50
docker run -it --name myubuntu ubuntu_py3:20.04 /bin/bash

### 挂载
docker run -it -v E:\docker:/home/project ubuntu_py3:20.04

### 直接进入
docker exec -it myubuntu1 /bin/bash

### 重新启动
docker restart myubuntu1

### 安装依赖
pip install -r requirements.txt

## ubuntu内部代码

### 编辑代码
vim xxx.py

### 新建文件
touch xxx.py

### 运行python文件
python xxx.py



### 设置中文
https://blog.csdn.net/HELLOWORLD2424/article/details/128442204

### 安装python
get-apt python/python3

### # coding:utf-8



## docker镜像加速器
  "registry-mirrors": [
    "https://hub-mirror.c.163.com",
    "https://mirror.baidubce.com"
  ]