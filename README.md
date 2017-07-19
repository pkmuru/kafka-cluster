
https://mythinkpond.com/2016/03/23/centos-7-how-to-open-ports-in-firewalld/


iptables -nL --line-numbers
netstat -tulpn

### add port

> sudo firewall-cmd --zone=public --add-port=8080/tcp --permanent

> sudo firewall-cmd --reload

kafka-manager 9000
zookeeper 2181


### Zookeeper
>bin/zookeeper-server-start.sh -daemon config/zookeeper.properties


### Kafka Server
> bin/kafka-server-start.sh config/server.properties
 

### kafka-manager

> bin/kafka-manager -Dconfig.file=/opt/kafka-manager-1.3.3.8/conf/application.conf



