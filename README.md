
# Setting Up Confluent Kafka 3.0.0

<p>

- Make sure you are navigated inside the bin/windows directory.

## Start Zookeeper and Kafka Broker

-   Start Zookeeper

```
zookeeper-server-start.bat ..\..\etc\kafka\zookeeper.properties
```

-   Start Kafka Broker

```
kafka-server-start.bat ..\..\etc\kafka\server.properties
```
