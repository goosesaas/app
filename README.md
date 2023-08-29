# kafka
training about kafka
```console
$ get https://downloads.apache.org/kafka/3.5.0/kafka_2.12-3.5.0.tgz
```
Extract it using the below command
```console
$ tar -xf kafka_2.12-3.5.0.tgz
```
CD in to the folder
```console
$ cd kafka_2.12-3.5.0/
```
Start the ZOOkeeper
```console
$ nohup sh bin/zookeeper-server-start.sh config/server.properties > zk.log &
```
Check the Zookeeper server
```console
$ telnet localhost 2181
```
Start Kafka server
```console
$ nohup sh bin/kafka-server-start.sh config/server.properties > zk.log &
```
Check the Kafka server
```console
$ telnet localhost 9002
```
List topics
```console
$ sh bin/kafka-topics.sh --bootstrap-server localhost:9092 --list
```
Create  topics
```console
$ bin/kafka-topics.sh --bootstrap-server localhost:9092 --topic learningKafka -create
```
Creating a topic producer
```console
$ sh bin/kafka-console-producer.sh --broker-list localhost:9092 --topic kafkatopic
```
creating a consumer
```console
$ sh bin/kafka-console-consumer.sh  --bootstrap-server localhost:9092 --topic kafkatopic
```
alter config for retention time interval
```console
$ bin/kafka-configs.sh --bootstrap-server localhost:9092 --entity-type topics --entity-name kafkatopic --alter --add-config retention.ms=2000
```
list the config of a topic 
```console
$ bin/kafka-topics.sh --bootstrap-server localhost:9092 --describe --topic kafkatopic
```
after updating the retention time we have to execute the consumer from begining 
```console
$ sh bin/kafka-console-consumer.sh  --bootstrap-server localhost:9092 --topic kafkatopic --from-begining
```

Configuring https://cloud.mongodb.com 
![image](https://github.com/goosesaas/app/assets/143482065/4756a4f1-59bf-4d6a-94c4-aba5c765cd9b)


to get the host name

![image](https://github.com/goosesaas/app/assets/143482065/16fe2d53-fd6c-4ba4-ba91-b05e8532000d)


hree is the API KEY

```
=== Confluent Cloud API key: lkc-5m1njq ===

API key:
ZVITDG4LHZN7PSWK

API secret:
UQnLEuZD7jEpMEXWpm+gV56mjHS5D3EolwSAZUecPKNYoeFD4aPWvUM6l6LVJJu9

Bootstrap server:
pkc-lzvrd.us-west4.gcp.confluent.cloud:9092
```
after the details you have to see this. https://confluent.cloud/

![image](https://github.com/goosesaas/app/assets/143482065/6327bf54-9ff6-48d5-b5b7-d6f6d36b9db0)


Home
Environments
default
cluster_0
Connectors
MongoDbAtlasSourceConnector_2

![image](https://github.com/goosesaas/app/assets/143482065/2757bd2b-e3e3-4bd3-bcc2-01e933892a24)




Mongo DB with Node JS and Express

```console
npm install express express-graphql graphql mongoose
```
after create a folder add app.js/db.js/package.js and schema.js in one folder and run the below command

```console
npm install
```

[Cloudflare CDN ](https://dash.cloudflare.com/profile)

![image](https://github.com/goosesaas/app/assets/143482065/b8b5ca76-c53d-4308-9ae6-7abd9bfa4a83)


