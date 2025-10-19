
## use in terminal for interact with kafka container
```sh
docker exec -it name_of_container bash  

docker exec -it kafka bash  
```


# creation of topics
```sh
kafka-topics --create --topic test-topic --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
```

# list topics
```sh
kafka-topics --list --bootstrap-server localhost:9092
```


# create messages
```sh
kafka-console-producer --topic test-topic --bootstrap-server localhost:9092
```
-  then write the message, after that use ctrl-c to close program.


# in another console use, to read the messages
```sh
kafka-console-consumer --topic test-topic --bootstrap-server localhost:9092 --from-beginning
```



#### NOTE
when images form confluentinc are usded isnt necesary use .sh extension:
Use kafka-topics instead kafka-topics.sh in bash commands
