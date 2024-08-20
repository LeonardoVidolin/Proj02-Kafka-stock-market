# Proj02-Kafka-stock-market

## Introduction

This project is an End-to-End Data Engineering solution designed to process real-time stock market data using Apache Kafka. The primary goal is to practice and demonstrate proficiency with various data engineering tools and technologies. By working through this project, you will gain hands-on experience with real-time data streaming, data storage, processing, and querying in a scalable environment.

## Project Overview

In this project, we are simulating a real-world data engineering pipeline that handles continuous streams of stock market data. The data flows through a Kafka topic, where it is ingested and processed before being stored in Amazon S3. From there, AWS Glue Crawlers and the Glue Catalog are used to prepare the data for querying in Amazon Athena. The overall architecture is designed to be scalable, robust, and efficient, making it a practical exercise for learning key data engineering concepts.

## Architecture



## Technology Stack

Programming Language: Python
Amazon Web Services (AWS):
S3 (Simple Storage Service): For storing the processed data.
Athena: For querying the data stored in S3.
Glue Crawler: For cataloging the data in S3.
Glue Catalog: To maintain the metadata of the data stored in S3.
EC2: For hosting the Kafka broker and other necessary components.
Apache Kafka: For real-time data streaming and ingestion.

## Objective

The main objective of this project is to train with and showcase your skills in real-time data engineering, using a variety of tools and technologies. It serves as a hands-on demonstration of how these technologies can be integrated to create a complete data pipeline that handles streaming data efficiently.

## Dataset Used

Here is the dataset used - https://github.com/darshilparmar/stock-market-kafka-data-engineering-project/blob/main/indexProcessed.csv
