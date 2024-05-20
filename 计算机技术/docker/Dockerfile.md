# Dockerfile

 # ubuntu_py3:20.04
 # docker build -f Dockerfile-u20py3 -t ubuntu_py3:20.04 .


FROM ubuntu:20.04

#更换下载源,下载安装python3(3.8) 更换后很慢？
#COPY sources.list /etc/apt/
#RUN apt-get update && apt-get upgrade -y && apt-get install -y libssl-dev python3-pip curl inetutils-ping vim --fix-missing
#RUN pip3 install --upgrade pip

#删除不必要的dev包以减小Image大小
#RUN apt-get -y purge *-dev

#安装python依赖包
#COPY requirements.txt /
#RUN pip3 install -r requirements.txt -i https://pypi.douban.com/simple && rm requirements.txt

