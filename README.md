# Docker_kafka

### Change IP address in the docker-compose.yml fileaccording to your machine ip address
```
KAFKA_ADVERTISED_LISTENERS: PLAINTEXT://192.168.70.170:9092
```
### Get the zookeeper console
```docker exec -it wurstmeister/zookeeper sh```
### Then Run the following command
```
./bin/zkCli.sh
create /kafka-manager/mutex ""Created /kafka-manager/mutex
create /kafka-manager/mutex/locks ""Created /kafka-manager/mutex/locks
create /kafka-manager/mutex/leases ""Created /kafka-manager/mutex/leases
```


start zookeeper (port:2181):
```bin/zookeeper-server-start.sh config/zookeeper.properties```

start kafka (Port 9092):
```bin/kafka-server-start.sh config/server.properties```

create kafka topic: 
```bin/kafka-topics.sh --create --topic mytopic --bootstrap-server localhost:9092```
bin/kafka-topics.sh --create --topic mytopic --partitions 1 --replication-factor 1 --bootstrap-server localhost:9092


start console producer: 
```bin/kafka-console-producer.sh --topic mytopic  --bootstrap-server localhost:9092```
//enter msg//

start console consumer: 
```bin/kafka-console-comsumer.sh --topic mytopic --bootstrap-server localhost:9092```
//it will show here//
