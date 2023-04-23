# Kafka-Big-Data

# Kafka Project
This project provides an example of how to use Kafka to send and receive messages.

## Step 1: Install Kafka and Zookeeper
First, you need to install Kafka and Zookeeper. Here are the steps:  
1. Download Kafka and Zookeeper from the official website.   
     1.1. Download Kafka from the Apache Kafka website: https://kafka.apache.org/downloads.  
     1.2. Download Zookeeper from the Apache Zookeeper website: https://zookeeper.apache.org/.
2. Extract the files to a directory on your computer.
3. Open a terminal window and navigate to the directory where Kafka and Zookeeper are located.
4. Start Zookeeper by running the following command: ./bin/zookeeper-server-start.sh config/zookeeper.properties
5. Start Kafka by running the following command: ./bin/kafka-server-start.sh config/server.properties

## Step 2: Create a Kafka Topic
1. Open a new terminal window and navigate to the directory where Kafka is located.
2. Create a new topic by running the following command: ./bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic topic_1

## Step 3: Run the Producer and Consumer
1. Producer: .\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic topic_1
2. Consumer: .\bin\windows\kafka-topics.bat --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic topic_1
