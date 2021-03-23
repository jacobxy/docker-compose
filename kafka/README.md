# kafka 操作
[链接](https://blog.csdn.net/qq_26375325/article/details/105251205)

## 创建topic

```
kafka-topics.sh --create --topic test \
--zookeeper zookeeper:2181 --replication-factor 1 \
--partitions 1
```

## 生产者发送消息

```
kafka-console-producer.sh --topic=test --broker-list kafka:9092
```

## 消费者接收消息

```
kafka-console-consumer.sh --bootstrap-server kafka:9092 --from-beginning --topic test
```


