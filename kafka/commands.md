## Kafka Console Producer-Consumer

- Create new topic:`kafka-topics --create --bootstrap-server localhost:9092 --topic <topic_name>`
- List Topics: `kafka-topics --list --bootstrap-server localhost:9092`
- Start consumer: `kafka-console-consumer --bootstrap-server  localhost:9092 --topic <topic_name>`
- Start console producer and produce messages on the topic: `kafka-console-producer --broker-list localhost:9092 --topic <topic_name>`
- Start console producer and produce messages in `key:value` pairs: `kafka-console-producer --broker-list localhost:9092 --topic <topic_name> --property "parse.key=true" --property "key.separator=:"`
