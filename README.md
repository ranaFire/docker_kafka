# docker_kafka

### Change IP address according to your machine ip address
### Get the zookeeper console
```docker exec -it zookeeper sh```
### Then Run the following command
```
./bin/zkCli.sh
create /kafka-manager/mutex ""Created /kafka-manager/mutex
create /kafka-manager/mutex/locks ""Created /kafka-manager/mutex/locks
create /kafka-manager/mutex/leases ""Created /kafka-manager/mutex/leases
```
