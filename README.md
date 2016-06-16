# Zookeeper

- Installation:

- cd /opt
- wget http://apache-mirror.rbc.ru/pub/apache/zookeeper/zookeeper-3.4.6/zookeeper-3.4.6.tar.gz
- gunzip -c *gz | tar xvf -
- cd zookeeper-3.4.6/conf

- cp zoo_sample.cfg zoo.cfg
- vim /opt/zookeeper-3.4.6/bin/zkServer.sh
- chmod -R 750 /opt/zookeeper-3.4.6
 
- export ZOOCFGDIR=/opt/zookeeper-3.4.6/conf
- export ZOOCFG=zoo.cfg
- ./zkServer.sh start

- This runs zookeeper on port 2181
 
- testing:
- netstat -tulpn | grep :2181
