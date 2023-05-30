# Module 17 AWS and PySpark

# Amazon_Vine_Analysis

## Overview of the Analysis

Using the starter code provided, this challenge is to produce analysis results for product reviews on Vine. The objective is to learn how to import tables to AWS Postgres DB from text files stored on S3. Then perform analysis of the data using Pyspark in a Google Collab notebook.

## Analysis Results

After filtering the data to reviews that had at least 20 votes and at least 50% helpful votes, there were 14537 reviews in the analysis. 
- Several customers are frequent reviewers, with 20 or more reviews.
- The Vine reviews are paid reviews whereas the others are unpaid. 
- Of the 14537 reviews, 8246 are 5-star reviews.
- The vast majority of the 5-star reviews are unpaid. The table below shows the breakdown of the 5-star reviews.


---

![Count of Reviews by Customer ID ](/Resources/reviewspercustomer.png)

---

![Vine Versus non-Vine Reviews](/Resources/paidvsunpaid.png)

---
## Summary

This analysis did not show any positivity bias for reviews in the Vine program, at least for 5-star reviews. It would be interesting to compare the breakdown at each star rating of Vine versus non-Vine reviews to see if there are any trends. Also, I did not examine if the customers who had at least 20 reviews had a different distribution compared to other reviewers combined.  It's possible that they can intentionally skew the overall rating by reviewing repeatedly.