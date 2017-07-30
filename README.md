# datasic
## 简介
机器学习、数据分析，开发、运行环境
## 本镜像包含
* python3
* jupyter
* tensorflow
* numpy
* scipy
* matplotlib
* pandas
* sympy
* nose

## 如何运行
运行以下脚本，创建容器
```
# 以下变量可以自己定义
Image=transferx/datasic
Container=datasic_c
Volume=/media/sf_e

sudo docker run -d -P -v $Volume:/src --name $Container $Image
sudo docker ps | grep $Container
```
这是会输出以下内容：
`a4ab3b133e94        transferx/datasic    "/bin/sh -c 'jupyter "   About an hour ago   Up About an hour    0.0.0.0:32771->8888/tcp    datasic_c`
通过`0.0.0.0:32771`即可以访问jupter（注意这里的ip和端口因个人而已）。
登录密码：jupyter
