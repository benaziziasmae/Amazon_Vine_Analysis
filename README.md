# Amazon_Vine_Analysis
Amazon_Vine_Analysis


## Overview of the project

This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.

We focused our analysis on the US reviews for kitchen.


## Resources
- Data : [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
- Software : Google Colab Notebook, PostgreSQL, pgAdmin 4, Amazon Web Service AWS

## Summary 

### 1- Deliverable 1

![Customer_table](/Resources/Customer_table.PNG)

![Product_table](/Resources/Product_table.PNG)

![Review_ID_table](/Resources/Review_ID_table.PNG)

![vine_table](/Resources/vine_table.PNG)



### 2- Deliverable 2

![total_vote](/Resources/total_vote.PNG)

![helpful_vote](/Resources/helpful_vote.PNG)

![vine_y](/Resources/vine_y.PNG)

![vine_n](/Resources/vine_n.PNG)


### 3- Deliverable 3

![total_paid_reviews](/Resources/total_paid_reviews.PNG)

![five_star_Reviews%](/Resources/five_star_Reviews%.PNG)

