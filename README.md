# Kafka

# Introduction

![](https://github.com/shamy1st/kafka/blob/main/images/01-how-companies-start.png)

![](https://github.com/shamy1st/kafka/blob/main/images/02-after-a-while.png)

![](https://github.com/shamy1st/kafka/blob/main/images/03-organizations-facing-problems.png)

![](https://github.com/shamy1st/kafka/blob/main/images/04-why-apache-kafka.png)

![](https://github.com/shamy1st/kafka/blob/main/images/05-why-apache-kafka.png)

![](https://github.com/shamy1st/kafka/blob/main/images/06-why-apache-kafka.png)

![](https://github.com/shamy1st/kafka/blob/main/images/07-apache-kafka-use-cases.png)

![](https://github.com/shamy1st/kafka/blob/main/images/08-apache-kafka-examples.png)

![](https://github.com/shamy1st/kafka/blob/main/images/09-course-structure.png)

# Kafka Fundamentals

## Kafka Theory

### Topics, Partitions and Offsets

![](https://github.com/shamy1st/kafka/blob/main/images/01-topics.png)

![](https://github.com/shamy1st/kafka/blob/main/images/02-topics.png)

![](https://github.com/shamy1st/kafka/blob/main/images/03-topics.png)

### Brokers and Topics

![](https://github.com/shamy1st/kafka/blob/main/images/01-brokers.png)

![](https://github.com/shamy1st/kafka/blob/main/images/02-brokers.png)

### Topic Replication

![](https://github.com/shamy1st/kafka/blob/main/images/01-topic-replication.png)

![](https://github.com/shamy1st/kafka/blob/main/images/02-topic-replication.png)

![](https://github.com/shamy1st/kafka/blob/main/images/03-topic-replication.png)

### Producers and Message Keys

![](https://github.com/shamy1st/kafka/blob/main/images/01-producers.png)

![](https://github.com/shamy1st/kafka/blob/main/images/01-producers.png)

![](https://github.com/shamy1st/kafka/blob/main/images/01-producers.png)

### Consumers & Consumer Groups

![](https://github.com/shamy1st/kafka/blob/main/images/01-consumers.png)

![](https://github.com/shamy1st/kafka/blob/main/images/02-consumers.png)

![](https://github.com/shamy1st/kafka/blob/main/images/03-consumers.png)

### Consumer Offsets & Delivery Semantics

![](https://github.com/shamy1st/kafka/blob/main/images/01-consumer-offsets.png)

![](https://github.com/shamy1st/kafka/blob/main/images/02-consumer-offsets.png)

### Kafka Broker Discovery

![](https://github.com/shamy1st/kafka/blob/main/images/broker-discovery.png)

### Zookeeper

![](https://github.com/shamy1st/kafka/blob/main/images/01-zookeeper.png)

![](https://github.com/shamy1st/kafka/blob/main/images/02-zookeeper.png)

### Kafka Guarantees

![](https://github.com/shamy1st/kafka/blob/main/images/kafka-guarantees.png)

### Theory Roundup

![](https://github.com/shamy1st/kafka/blob/main/images/theory-roundup.png)


## Starting Kafka

### Mac - Install using PATH

* https://kafka.apache.org/downloads
* Binary downloads:
* Then download, then extract binaries to a specific directory
* \> cd bin
* \> brew tap caskroom/versions
* \> brew cask install java8
* you need java8, not java9, not java10, not java11 for now.
* \> /installation/kafka_2.13-2.7.0/bin/kafka-topics.sh
* \> cat ~/.bash_profile 
* \> nano ~/.bash_profile
* add kafka binaries path

### Mac - Install using brew

* \> brew install kafka

### Mac - Start Zookeeper and Kafka

* modify dataDir=installation/data/zookeeper in config/zookeeper.properties
* \> nano installation/config/zookeeper.properties
* start zookeeper server
* \> installation/bin/zookeeper-server-start.sh installation/config/zookeeper.properties

* modify log.dirs=installation/data/kafka in config/server.properties
* \> nano installation/config/server.properties
* start kafka
* \> installation/bin/kafka-server-start.sh installation/config/server.properties

## CLI (Command Line Interface) 101

### Create Topic

![](https://github.com/shamy1st/kafka/blob/main/images/cli-create-topic.png)

### Delete Topic

![](https://github.com/shamy1st/kafka/blob/main/images/cli-delete-topic.png)

### Producer

![](https://github.com/shamy1st/kafka/blob/main/images/cli-producer.png)

![](https://github.com/shamy1st/kafka/blob/main/images/cli-producer-change-default.png)

![](https://github.com/shamy1st/kafka/blob/main/images/cli-producer-change-default-2.png)

### Consumer

* will consume only real-time when you start to consume

![](https://github.com/shamy1st/kafka/blob/main/images/cli-consumer.png)

* from begging will consume the topic from the begging till now + real-time

![](https://github.com/shamy1st/kafka/blob/main/images/cli-consumer-from-begging.png)

### Consumer in Group

* the producers load will distribute over the consumers
* if one of the consumers fail, the load will be distributed to others
* if you close the consumer group command and start it again, it will start where it stopped because the offset is resetted

![](https://github.com/shamy1st/kafka/blob/main/images/cli-consumer-in-group.png)

![](https://github.com/shamy1st/kafka/blob/main/images/cli-consumer-in-group-2.png)

### kafka-consumer-groups

![](https://github.com/shamy1st/kafka/blob/main/images/cli-kafka-consumer-groups.png)

### Resetting Offsets



### Kafka Tools UI



# Kafka Real World Project


# Kafka Ecosystem & Real-World Architectures


# Advanced Kafka


# Annexes


## Ref
* https://www.udemy.com/course/apache-kafka/
