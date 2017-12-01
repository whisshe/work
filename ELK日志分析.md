### ELK简介
ELK stack是实时日志处理领域开源的一套解决方案
E代表Elasticsearch,负责日志的存储和检索； 
L代表Logstash, 负责日志的收集，过滤和格式化； 
K代表Kibana，负责日志的展示统计和数据可视化
### 架构图
![Image text](https://raw.githubusercontent.com/whisshe/work/master/ELK.png)
### 安装过程
- 安装Java
```
echo "deb http://ppa.launchpad.net/webupd8team/java/ubuntu trusty main" >> /etc/apt/sources.list
echo "deb-src http://ppa.launchpad.net/webupd8team/java/ubuntu trusty main" >> /etc/apt/sources.list
apt-key adv --keyserver keyserver.ubuntu.com --recv-keys EEA14886
apt-get update
apt-get install oracle-java8-installer
apt install oracle-java8-set-default
```
### 下载ELK
```
wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-6.0.0.tar.gz
wget https://artifacts.elastic.co/downloads/logstash/logstash-6.0.0.tar.gz
wget https://artifacts.elastic.co/downloads/kibana/kibana-6.0.0-linux-x86_64.tar.gz
```