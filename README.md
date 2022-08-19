# Module 16: Big Data

## Overview of the Analysis

### Purpose
The purpose of this challenge was to analyze the reviews for Video Games sold on Amazon. Using PySpark, the reviews were **extracted** from the [Amazon Customer Reviews Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), **transformed** into four seperate dataframes, connected to an AWS RDS instance, and **loaded** into a PostgreSQL database. Then, an analysis was performed to determine if there is any bias from Amazon Vine members for favourable reviews. 

### Resources
* Amazon RDS
* Google Colab, PySpark
* pgAdmin, PostgreSQL
* Challenge Code: [Amazon_Reviews_ETL.ipynb](https://github.com/daniel-sh-au/UofT_DataBC_Module16_Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb), [Vine_Review_Analysis.ipynb](https://github.com/daniel-sh-au/UofT_DataBC_Module16_Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)

## Results
![results.png](https://github.com/daniel-sh-au/UofT_DataBC_Module16_Amazon_Vine_Analysis/blob/main/Resources/results.png)  
* There were **90** Vine reviews and **37,385** non-Vine reviews
* There were **44** 5-star Vine reviews and **14,626** 5-star non-Vine reviews
* **48.89%** of Vine reviews were 5-stars and **39.12%** of non-Vine reviews were 5 stars

From the results, there were significantly more non-Vine reviews than Vine reviews. This pattern was also observed in the count of 5-star reviews for non-Vine and Vine reviews. However, the percent of 5-star Vine reviews was approximately 10% more than the percent of 5-star non-Vine reviews, revealing some potential bias. 

## Summary
From the results, it was found that the percentage of 5-star reviews from Vine members was about 10% higher than the percentage of 5-star reviews from non-Vine members. This value suggest positivity bias for reviews from Vine members. Additional analysis could be performed to support this statement from the other columns in the original dataset. Review_headline and review_body could be analyzed with the Natural Language Processing pipeline for further insight from comments left by Vine and non-Vine customers.  

![further_analysis_reviews.png](https://github.com/daniel-sh-au/UofT_DataBC_Module16_Amazon_Vine_Analysis/blob/main/Resources/further_analysis_reviews.png)