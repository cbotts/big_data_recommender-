# Big Data Recommender
 Recommender system with big data tools

 ## Objective 
 Utilize big data tools to process a large volume of data. Create a recommender based on commonly purchased products that suggests add on items in real time.

 ## How to Run 
 ```
git clone https://github.com/cbotts/big_data_recommender-/
open Botts_DSC650_Final.pdf
```

## Data 
Data Source: carrie1 on Kaggle 
https://www.kaggle.com/datasets/carrie1/ecommerce-data

The data used to build this big data pipeline is a large collection of retail transactions.

## Methods 
This project utilized Apache NiFi, Solr, HDFS, and Kafka. 
A pipeline was built in NiFi which ingested transactional data. Original records were stored in HDFS and Solr was used to query transaction information. The query results were published to Kafka so that they could be viewed in the Kafka consumer terminal. NiFi processors were used to preprocess data as necessary for storage, querying, and record conversion. 

A csv file was used for proof of concept, but for real time processing, transaction data could be collected by Kafka and then ingested by NiFi. 

## Conclusion 
Solr is a powerful search engine and can perform advanced queries to generate specific outputs for a recommender system. NiFi can be used to create an effective workflow. Integration of Apache Spark would enable machine learning to further improve the recommender system. 
