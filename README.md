KafkaStormHbase
===============

Install a cluster to try summingbird

Install zookeeper
=================

Download from http://zookeeper.apache.org/releases.html




Install Storm
=============

Source: http://www.thecloudavenue.com/2013/11/InstallingAndConfiguringStormOnUbuntu.html


wget http://download.zeromq.org/zeromq-2.1.7.tar.gz

---tar -xzf zeromq-2.1.7.tar.gz

cd zeromq-2.1.7

./configure

make

sudo make install

sudo apt-get install libtool git


Download storm from http://storm-project.net/downloads.html

By example :

wget https://dl.dropboxusercontent.com/s/tqdpoif32gufapo/storm-0.9.0.1.tar.gz

Configure Storm memmory

For low memmory

export STORM_JAR_JVM_OPTS="-Xmx64M -Xms32M"


Create a folder called data in the extracted folder.

- Modify the conf/storm.yaml file


Configure for you machine, if it is localhost

storm.zookeeper.servers:
- "192.168.19.161"
 
storm.local.dir: "/home/vm4learning/Installations/storm-0.8.2/data"
nimbus.host: "192.168.19.161"
supervisor.slots.ports:
- 6700
- 6701






Install Kafka
=============
Configure Storm

Configure Kafka

