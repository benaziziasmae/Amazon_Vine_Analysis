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

- Loaded the DataFrames that correspond to tables in pgAdmin.

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

In this deliverable, we will determine if there is any bias towards reviews that were written as part of the Vine program. and we will determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

We followed the according steps:

- Filtered the data and create a new DataFrame or table to retrieve amany information regarding the reviwes: total vote=>20, helpful vote, vine =='y', vine=='n'..
- Determined the number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for the two types of review (paid vs unpaid).

And the results showed as the following:

![total_vote](/Resources/total_vote.PNG)

![helpful_vote](/Resources/helpful_vote.PNG)

![vine_y](/Resources/vine_y.PNG)

![vine_n](/Resources/vine_n.PNG)

![total_paid_reviews](/Resources/total_paid_reviews.PNG)

![five_star_Reviews](/Resources/five_star_Reviews.PNG)

![total_unpaid_reviews](/Resources/total_unpaid_reviews.PNG)

![unpaid_five_star_reviews](/Resources/unpaid_five_star_reviews.PNG)

### 3- Deliverable 3/ Results and Analysis:

In this section we wil do a breive summary/analysis about the results we got from deliverable 1 and 2.

### Results
For the kitchen review that we selected, the results show like the following:

**Paid Reviews**

- 1207 total paid reviews.
- with 509 total of paid five start reviews, 
- giving a percentage of 42%.


**Unpaid Reviews**
- 97839 total paid reviews.
- with 45858 total of paid five start reviews, 
- giving a percentage of about 47%.

### Analysis

- 42% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 47%.
- Also, the total review in the unpaid vine program were more important that the paid program.
- That's to say, and as per the percentage calculated, we can conclude that analysis the vine program does not show any big bias.
- Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.
