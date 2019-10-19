
#### Application Configurations

1- setup <ip-address:port> in `server.properties`
```
    Properties properties=new Properties();
    {
    	properties.put("bootstrap.servers", "<ip-address:port>");
    	properties.put("key.serializer", "org.apache.kafka.common.serialization.StringSerializer");
    	properties.put("value.serializer", "org.apache.kafka.common.serialization.StringSerializer");
    }
```


#### Kafka Configurations

- zookeeper.properties (No change)
- server.properties
```
    #listeners = PLAINTEXT://your.host.name:9092
    listeners=PLAINTEXT://<ip-address-of-the-machine>:9092
    
    #advertised.listeners=PLAINTEXT://your.host.name:9092
    advertised.listeners=PLAINTEXT://<ip-address-of-the-machine>:9092
    
    #kafka commit logs directory
    log.dirs=/tmp/kafka-logs
```
- consumer.properties
```
    #bootstrap.servers=localhost:9092
    bootstrap.servers=10.0.0.69:9092
```
- producer.properties
```
    #bootstrap.servers=localhost:9092
    bootstrap.servers=10.0.0.69:9092
```
