# Module 16 Challenge

---
## Amazon Vine Analysis
---

## Project Overview
As a data expert at BigMarket, a start up that helps buisinesses optimize their marketing efforts, your client is about to release a large catelog of products on a retail website and has hired you to analyize how product reviews will likely impact their business. Specifically, they are interested in how reviews of their products compare to similar products of their competitors, and if the Vine program, that gives free products to consumers who are then required to write a review of the product, is worth the cost. 

## Challenge Objectives
This project analyzes Amazon reviews of lawn and garden products written by members of the paid Amazon Vine program to determine if there is a bias toward favorable reviews from Vine members. The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and complete the analysis of the reviews.\

## Resources
**Data Sources:** 
- [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
- [Lawn and Garden Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Lawn_and_Garden_v1_00.tsv.gz)

**Software:**
- Google Colab Notebook
- PostgreSQL 12.0.9
- pgAdmin 4
- AWS

## Results
### Size of the Data Set
How many Vine reviews and non-Vine reviews were in the data set?
- Total Number of Vine Reviews <p align="center">
    <img src="https://github.com/saraegregg/Mod16_BigData/blob/main/images/total_paid_reviews.png"> 
</p>

<br>

- Total Number of Non-Vine Reviews <p align="center">
    <img src="https://github.com/saraegregg/Mod16_BigData/blob/main/images/total_unpaid_reviews.png"> 
</p>
<br>

### 5-Star Reviews
How many Vine reviews were 5-stars? How many non-Vine reviews were 5 stars?
- Total Number of Vine Reviews That Awarded 5 Stars <p align="center">
    <img src="https://github.com/saraegregg/Mod16_BigData/blob/main/images/fivestar_paid_reviews.png"> 
</p>

<br>

- Total Number of Non-Vine Reviews That Awarded 5 Stars <p align="center">
    <img src="https://github.com/saraegregg/Mod16_BigData/blob/main/images/fivestar_unpaid_reviews.png"> 
</p>
<br>

### 5-Star Review Percents
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- Percentage of Vine Reviews That Awarded 5 Stars <p align="center">
    <img src="https://github.com/saraegregg/Mod16_BigData/blob/main/images/percentage_paid_fivestar_reviews.png"> 
</p>

<br>

- Percentage Non-Vine Reviews That Awarded 5 Stars <p align="center">
    <img src="https://github.com/saraegregg/Mod16_BigData/blob/main/images/percentage_unpaid_fivestar_reviews.png"> 
</p>
<br>

## Summary
51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program.\
Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.