
# Setting Up Confluent Kafka 3.0.0

<p>

- Make sure you are inside the bin/windows directory of Kafka Confluent distribution.

## Start Everything all at once

```
confluent local services start
```

## Start Zookeeper and Kafka Broker
  
-   Start Both at once

```
confluent local services kafka start
```

-   Start Zookeeper

```
$CONFLUENT_HOME/bin/zookeeper-server-start $CONFLUENT_HOME/etc/kafka/zookeeper.properties
```

-   Start Kafka Broker

```
$CONFLUENT_HOME/bin/kafka-server-start $CONFLUENT_HOME/etc/kafka/server.properties
```

-   Start Schema Registry

```
$CONFLUENT_HOME/bin/schema-registry-start $CONFLUENT_HOME/etc/schema-registry/schema-registry.properties
```
  
OR

```
confluent local services schema-registry start
```

-   Start Control Center

```
$CONFLUENT_HOME/bin/control-center-start $CONFLUENT_HOME/etc/confluent-control-center/control-center.properties
```

## Other Confluent Commands
  
-   Service Status

```
confluent local services status
```
  
-   Stop Services

```
confluent local services stop
```
  
-   Start Control Center

```
confluent local services control-center start
```

-   Clean Up all Confluent temp files and data

```
confluent local destroy
```
