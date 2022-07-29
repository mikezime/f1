## Topics
similar to tables in db,they are split into partitions, consists of Topic/Partition/Offset

## Broker
 server in a cluster.only one broker can be leader, only one leader can receive or serve data , usually 3 brokers can be up to 100

## Topic replication factor
 >1 (usually 2 or 3 )

## Who sync data
Brokers will sync data

## Producers
 writes data. 

## Data received acks
writing acknowledge can be : 0,1-default,all

## Key
truck_id for example (for truck tracking app)

## Consumers
 read the data

## Consumers Group
application

## Consumer offset
committed live by consumer into __consumer_offsets, consumer choose when to commit offset

## Delivery semantics
3 semantics: at most once (when msg received), at least once (when msg processed,preferred),exactly once => Kafka streams API (from kafka to kafka or from kafka to db)

## Broker discovery
every broker knows all about brokers,topics,partitions (metadata)

## Zookeper
manage brokers,kafka cannot work w/out Zookeper, Zookeper sends notification to kafka

## Kafka Gurantees 
 msgs stored and can be read in orders

## Zookeper start
  zookeeper-server-start.sh config/zookeeper.properties 

## Kafka start
 kafka-server-start.sh config/server.properties 

## Create topic
 kafka-topics.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" --create --partitions 3  --replication-factor 1

## List topic
 kafka-topics.sh --bootstrap-server 127.0.0.1:9092 --list

## Delete topic
 kafka-topics.sh --bootstrap-server 127.0.0.1:9092 --topic "second_topic" --delete  

## describe topic
 kafka-topics.sh --bootstrap-server 127.0.0.1:9092 --topic "second_topic" --describe  

## Producer CLI command 
 kafka-console-producer.sh  (run and check out required fields)

## Produce messages 
kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" 

## Produce messages w/acks 
kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" --producer-property acks=all 

## CLI Consumer 
kafka-console-consumer.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" 

## CLI Consumer All Messages 
kafka-console-consumer.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" --from-beginning  

## CLI Consumer Groups 
kafka-console-consumer.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" --group mygroup1

## CLI Consumer Group All Once 
kafka-console-consumer.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" --group mygroup2 --from-beginning  

## CLI Group list 
 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092  --list

## CLI Group describe 
 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092  --group mygroup1 --describe

## CLI Group re-receive all msgs
 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" --group mygroup1 --reset-offsets --to-earliest --execute

## CLI Group re-receive couple msgs
 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092 --topic "first_topic" --group mygroup1 --reset-offsets --shift-by -2 --execute

