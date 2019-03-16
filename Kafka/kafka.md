## Start Zookeeper
zookeeper-server-start.bat ./config/zookeeper.properties

## Start Kafka 
kafka-server-start.bat ./config/server.properties


kafka-topics.bat --zookeeper localhost:2181 --topic hello_topic --create --partitions 3 --replication-factor 1

kafka-topics.bat --zookeeper localhost:2181 --list

kafka-topics.bat --zookeeper localhost:2181 --topic hello_topic --describe

kafka-topics.bat --zookeeper localhost:2181 --topic --delete

kafka-console-producer --broker-list 127.0.0.1:9092 --topic hello_topic

kafka-console-producer --broker-list 127.0.0.1:9092 --topic hello_topic --producer-property acks=all

kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic hello_topic --from-beginning


kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic hello_topic --group my_first_app
kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic hello_topic --group my_first_app
kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic hello_topic --group my_first_app

kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic hello_topic --group my_second_app --from-beginning

kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic hello_topic --group my_third_app


kafka-consumer-groups --bootstrap-server localhost:9092 --list
kafka-consumer-groups --bootstrap-server localhost:9092 --describe --group my_first_app


kafka-consumer-groups --bootstrap-server localhost:9092 --group my_first_app --reset-offsets --shift-by -2 --execute --topic hello_topic