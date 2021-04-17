# Amazon_Vine_Analysis
Amazon_Vine_Analysis


## Overview of the project

This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.

In this project, i have picked a data set from Amazon reviews regarding kitchen.


## Resources
- Data : [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
- Software : Google Colab Notebook, PostgreSQL, pgAdmin 4, Amazon Web Service AWS

## Summary 

### 1- Deliverable 1

In this deliverable we did the following steps:

- Extracted the "kitchen" reviews dataset from the list of review datasets from AWS S3 bucket and loaded into a DataFrame.

- Conducted necessary Transformations of the extracted dataset to make sure that the DataFrames match in both data type and column name. This will fit the dataset into tables of the schema file.

- Loaded the DataFrames that correspond to tables into an AWS RDS instance.

and we got the following results

**Customer table**

![Customer_table](/Resources/Customer_table.PNG)

**Product table**

![Product_table](/Resources/Product_table.PNG)

**Review by ID table**

![Review_ID_table](/Resources/Review_ID_table.PNG)

**Vine table**

![vine_table](/Resources/vine_table.PNG)



### 2- Deliverable 2

![total_vote](/Resources/total_vote.PNG)

![helpful_vote](/Resources/helpful_vote.PNG)

![vine_y](/Resources/vine_y.PNG)

![vine_n](/Resources/vine_n.PNG)


### 3- Deliverable 3

![total_paid_reviews](/Resources/total_paid_reviews.PNG)

![five_star_Reviews](/Resources/five_star_Reviews.PNG)

![total_unpaid_reviews](/Resources/total_unpaid_reviews.PNG)

![unpaid_five_star_reviews](/Resources/unpaid_five_star_reviews.PNG)

