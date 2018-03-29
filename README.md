# Spark-搭建
Hadoop2.7.3+Spark2.1.0完全分布式集群搭建过程：https://www.cnblogs.com/zengxiaoliang/p/6478859.html
***
## Centos7安装Python3的方法
https://blog.csdn.net/u012804180/article/details/79081424
### /etc/profile
### #Python3 Path
### export PATH=/usr/local/python3/bin:$PATH
### export LD_LIBRARY_PATH=/usr/local/python3/lib:$LD_LIBRARY_PATH

***

## centos7 安装teamviewer 报错libQt5WebKitWidgets.so.5()(64bit)
https://blog.csdn.net/kenny_lz/article/details/78884603

***

## pip 清华源
https://mirrors.tuna.tsinghua.edu.cn/help/pypi/

***

## pip 安装指定版本的包 

pip install somepackage==X.X.X(版本号)
***

## spark读取文件
### 本地文件 file:///home/z/Desktop/README.md
### hdfs文件 hdfs://Master:9000/user/README.md
默认是从hdfs读取文件，也可以指定sc.textFile("路径").在路径前面加上hdfs://表示从hdfs文件系统上读
本地文件读取 sc.textFile("路径").在路径前面加上file:// 表示从本地文件系统读，如file:///home/user/spark/README.md
***

## 配置pyspark的python版本
### /etc/profile中更改 /spark/conf/spark-env.sh中更改运行时会报版本不同的错误
### #Pyspark Path
### export PYSPARK_PYTHON=python3
### export PYSPARK_DRIVER_PYTHON=ipython
### #export PYSPARK_DRIVER_PYTHON_OPTS="notebook"
