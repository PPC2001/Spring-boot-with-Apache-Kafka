# Spring-boot-with-Apache-Kafka
Created Location Update App using Kafka which contains deliveryboy which act as producer and enduser which act as consumer

Run the below Commands in CMD - 

# Start ZooKeeper
bin\windows\zookeeper-server-start.bat config\zookeeper.properties

# Start Kafka
bin\windows\kafka-server-start.bat config\server.properties
  
#To craete the topic
C:\Users\chava\kafka\bin>windows\kafka-topics.bat --create --topic user-topic --bootstrap-server localhost:9092

Created topic user-topic.

# To write a some events in the topic / To produce the messagaes in the topic
C:\Users\chava\kafka\bin>windows\kafka-console-producer.bat --topic user-topic --bootstrap-server localhost:9092
>Hii
>This is my first Messagaes

# To read the events in the topic / To consume the messages from the topic
C:\Users\chava\kafka\bin\windows>kafka-console-consumer.bat --topic user-topic --from-beginning --bootstrap-server localhost:9092
Hii
This is my first Messagaes

---------------------------
Live Location Update Project - 

![image](https://github.com/PPC2001/Spring-boot-with-Apache-Kafka/assets/107803628/bae1ae0c-23fc-4b6f-acfc-a417700a5d77)

Publishing topic using Postman - 

![WhatsApp Image 2023-11-18 at 3 07 14 PM](https://github.com/PPC2001/Spring-boot-with-Apache-Kafka/assets/107803628/1b16a817-e361-4603-b808-223660ec2424)

Consuming the topic through CMD - 

![WhatsApp Image 2023-11-18 at 3 18 37 PM](https://github.com/PPC2001/Spring-boot-with-Apache-Kafka/assets/107803628/fdf6e854-6425-40c2-a234-2ee7c295e92c)

Consuming the topic through app - 

![WhatsApp Image 2023-11-18 at 3 18 11 PM](https://github.com/PPC2001/Spring-boot-with-Apache-Kafka/assets/107803628/06222a58-4441-4cf3-a654-6c0b17c2248b)




