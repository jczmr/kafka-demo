# kafka-demo
for the use of Kafka in microservices

## Kafka Architecture & Components

## Kafka Components
* Producer
    * Publish message / events
* Consumer
    * Receive message / events
* Broker
    * The Kafka Broker is nothing but just a server. In simple word, A broker is just an intermediate entity that helps in message exchange between a producer and a consumer. 
* Cluster
    * There can be one or more brokers in the Kafka cluster.
* Topic
    * It specifies the category of the message or the classification of the message. Listeners can then just respond to the messages that belong to the topics the are listening on.
* Partitions
    * A topic can be split into different parts, to improve performance, this concept is called topic partitioning.
    Each part is called partition in Kafka terminology.
* Offset
    * In Kafka, a sequence number is assigned to each message in each partition of a Kafka topic. This sequence number is called Offset.
* Consumer Groups
    * To better manage the workload ralated to a topic, a group of consumer instances can be grouped in a single unit named as a Consumer Group, then each of this instance can be associated to a specific partition of a topic.
    
    (also review the concept of consumer rebalancing)

* Zookeeper
    * Zookeeper is a prerequisite for Kafka. Kafka is a distributed system, and it uses Zookeeper for coordination and to track the status of Kafka cluster nodes. It also keeps track of Kafka topics, partitions, offsets, etc.

