##### Installation and startup

1. Install JDK.

  > $sudo apt-get install openjdk-8-jdk

  find installation path command: readlink -f $(which java)

  Set JAVA_HOME
  > export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64

  Set PATH
  > export PATH=$PATH:/usr/lib/jvm/java-8-openjdk-amd64/bin


2. Install Apache Kafka.

3. Start Zookeper server.
  > $ bin/zookeeper-server-start.sh config/zookeeper.properties

4. Start Kafka server.
  > $bin/kafka-server-start.sh config/server.properties




##### Creation of Topics.

Creating a test topic
> bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic nevtest





