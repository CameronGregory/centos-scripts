centos-scripts
==============

A collection of useful scripts for centos.

##Kafka

A init script for kafka.  Modify the KAFKA_HOME and KAFKA_USER, then:
```bash
sudo cp init.d/kafka /etc/rc.d/init.d
sudo chmod 755 /etc/rc.d/init.d/kafka
chkconfig kafka on
/etc/rc.d/init.d/kafka start
```

##Zookeeper

A init script for zookeeper, that assumes it's installed as part of kafka.  Modify the ZOOKEEPER_HOME and ZOOKEEPER_USER, then:
```bash
sudo cp init.d/zookeeper /etc/rc.d/init.d
sudo chmod 755 /etc/rc.d/init.d/zookeeper
chkconfig zookeeper on
/etc/rc.d/init.d/zookeeper start
```
