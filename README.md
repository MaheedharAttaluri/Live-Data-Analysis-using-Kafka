# Live Data Extracting from API using Kafka
![Labor-Market-GDP-Prediction](/Architecture.jpeg)
**Tech Stack:** Python,Kafka, AWS (Lambda, S3, Crawler, Glue, Athena)

•	Stock prices are extracted in real-time using the Finhub API and streamed into Kafka. A custom Python script functions as a producer, efficiently 
  pushing the data into Kafka topics.

•	The data flow is managed by Kafka, supported by ZooKeeper, ensuring robust data handling. Both Kafka brokers and ZooKeeper are hosted on AWS EC2 
  instances to effectively manage the processing load.

•	After processing, the data is stored in AWS S3, providing a scalable and secure storage solution that acts as a data lake for further processing 
  and analysis.

•	AWS Glue catalogs the data in S3, creating searchable metadata and schemas. This structured data is then queried using Amazon Athena, allowing for 
  advanced SQL-based analysis directly from the data lake.`


