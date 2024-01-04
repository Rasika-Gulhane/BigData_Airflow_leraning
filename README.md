# BigData_Kafka_Airflow
Learning Kafka with Spark Streaming and Airflow
[[Apache Kafka blog](https://kafka.apache.org/quickstart)]

STEP 1: DOWNLOAD AND INSTALL KAFKA
[[Download](https://www.apache.org/dyn/closer.cgi?path=/kafka/3.6.1/kafka_2.13-3.6.1.tgz)]

STEP 2: START THE KAFKA ENVIRONMENT (use cmd prompt and go inside kafka folder)
Start the ZooKeeper service
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

Start the Kafka broker service
.\bin\windows\kafka-server-start.bat .\config\server.properties

STEP 3: CREATE A TOPIC TO STORE YOUR EVENTS
.\bin\windows\kafka-topics.bat --create --topic topic_demo --bootstrap-server localhost:9092

STEP 4: WRITE SOME EVENTS INTO THE TOPIC
.\bin\windows\kafka-console-producer.bat --topic topic_demo --bootstrap-server localhost:9092

STEP 5:  READ THE EVENTS
.\bin\windows\kafka-console-consumer.bat --topic topic_demo --from-beginning --bootstrap-server localhost:9092
hello world
topic demo

