# Amazon_Vine_Analysis
Apache Hadoop (Hadoop), mrjob library (python), Apache Spart (Spark), Pyspark, Google Colaboratory (Colab), Data Tokenization, PySpark Machine Learning (ML) library, AWS SQL database, AWS S3 data storage, Database CRUD (create, read, update, delete), AWS SQL ETL flow, Naïve Bayes Model (ML)

## Overview of the analysis
A large volume dataset (including all the customer reviews of online video game purchases) is collected from the Amazon S3 storage bucket for data processing/cleaning to determine if bias exists in Amazon reviews for being or not being the members of the paid Amazon Vine program. Data is processed using python PySpark and then gets loaded into AWS RDS instance Postgres for further relational analysis. The analysis below illustrates the existence of bias toward favorable reviews from Vine members from the dataset.  

## Results
- In total, there are 94 Vine reviews and 40471 non-Vine reviews.  
![total_review.PNG](image/total_review.PNG)  
- There are 48 Vine reviews that have five stars and 15663 non-Vine reviews that have five stars.  
![five_star_review.PNG](image/five_star_review.PNG)  
- The percentage of five_star Vine reviews is 51.0638% and the percentage of five_star non_Vine reviews is 38.7018%.  
![percentage.PNG](image/percentage.PNG)  

## Summary
From the results above, it is likely that bias exists in the Vine program as the percentage of five_star Vine reviews is more than 10% higher than that of five_star non-Vine reviews.  
An analysis can also be conducted on "verified purchase" to see if non-verified purchases from Vine program members tend to provide more five-star ratings compared to non-Vine program members.  
