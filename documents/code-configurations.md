
#### Application Configurations

1- Setup <ip-address:port> in `server.properties`
```
    Properties properties=new Properties();
    {
    	properties.put("bootstrap.servers", "<ip-address:port>");
    	properties.put("key.serializer", "org.apache.kafka.common.serialization.StringSerializer");
    	properties.put("value.serializer", "org.apache.kafka.common.serialization.StringSerializer");
    }
```


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
