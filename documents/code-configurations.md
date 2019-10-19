
#### Application Configurations

1- 


```
    Properties properties=new Properties();
    {
    	properties.put("bootstrap.servers", "<ip-address:port>");
    	properties.put("key.serializer", "org.apache.kafka.common.serialization.StringSerializer");
    	properties.put("value.serializer", "org.apache.kafka.common.serialization.StringSerializer");
    }
```
