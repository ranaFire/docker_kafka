# docker_kafka

### Change IP address according to your machine ip address
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
