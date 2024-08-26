# Proj02-Kafka-stock-market

## Introduction

This project is an End-to-End Data Engineering solution designed to process real-time stock market data using Apache Kafka. The primary goal is to practice and demonstrate proficiency with various data engineering tools and technologies. By working through this project, you will gain hands-on experience with real-time data streaming, data storage, processing, and querying in a scalable environment.

## Project Overview

In this project, we are simulating a real-world data engineering pipeline that handles continuous streams of stock market data. The data flows through a Kafka topic, where it is ingested and processed before being stored in Amazon S3. From there, AWS Glue Crawlers and the Glue Catalog are used to prepare the data for querying in Amazon Athena. The overall architecture is designed to be scalable, robust, and efficient, making it a practical exercise for learning key data engineering concepts.

## Architecture

![Architecture](https://github.com/user-attachments/assets/b706e496-b0b5-4c5d-8445-e6412a2410fb)


## Technology Stack

- Programming Language: Python
Amazon Web Services (AWS): 
- S3 (Simple Storage Service): For storing the processed data.
- Athena: For querying the data stored in S3.
- Glue Crawler: For cataloging the data in S3.
- Glue Catalog: To maintain the metadata of the data stored in S3.
- EC2: For hosting the Kafka broker and other necessary components.
- Apache Kafka: For real-time data streaming and ingestion.

## Steps

Process

Set up a Kafka server on an EC2 instance:

- Launch a free t2.micro AWS instance and connect to it using SSH.
- Download Kafka and Java on the instance.
- Access the EC2 instance from outside the network using the public IPv4 address listed in the AWS instance details.
- Start the Zookeeper and Kafka servers, each in a separate terminal.
- Add inbound security rules to allow connections.
- Create a topic and run the producer in another terminal.
- Start the consumer in a separate terminal.

I used a .csv  sample file with stock market data to simulate the incoming data on Kafka. The Producer will read this .csv and generate the data that the consumer will receive and save the processed data on Amazon S3

## Objective

The main objective of this project is to train with and showcase your skills in real-time data engineering, using a variety of tools and technologies. It serves as a hands-on demonstration of how these technologies can be integrated to create a complete data pipeline that handles streaming data efficiently.

## Dataset Used

Here is the dataset used - https://github.com/darshilparmar/stock-market-kafka-data-engineering-project/blob/main/indexProcessed.csv
