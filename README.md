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

## Summary
In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
