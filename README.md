# Stock Market Data Pipeline
### Overview
This project implements a scalable data pipeline for processing and analyzing stock market data using Apache Kafka and AWS services. The pipeline ingests data from a stock market application, streams it through Kafka hosted on Amazon EC2, and processes it using AWS S3, AWS Glue, and Amazon Athena for storage, crawling, transformation, and querying.

### Architecture
![stock-market-kafka](https://github.com/user-attachments/assets/fc2ddd54-326f-41db-b668-0410e6cdf0ee)

### Technology
Python: Used for data processing, Kafka integration (via libraries like kafka-python), automation (e.g., AWS SDK)

Apache Kafka: Handles real-time stock market data streaming, acts as a data pipeline, processes events, and ensures scalability.

EC2 Instance: Hosted on Amazon Linux 2. Connected via SSH.

S3: Stores JSON data files for processing.

Athena: Queries the crawled data with SQL, displaying stock market indices and prices.

Glue Crawler: crawls data from an S3 bucket, outputs to Database, and runs on-demand with IAM role


