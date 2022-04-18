# Amazon_Vine_Analysis
Big Data Analysis using PySpark and the ETL process to anaylze large data sets of amazon purchase reviews. AWS database and PostgreSQL tables using PgAdmin were used to analyse the video game product dataset. 

## Resources 
Amazon Web Services (RDS), PgAdmin4, PySpark, Google Colab Notebook.
* Data Sources: [Amazon Product Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
* Specific product dataset used in this analysis: [Video Games](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)

## Overview
The purpose of this analysis is to assess Amazon product reviews written by members of the paid Amazon Vine program, specifically, video game products. Any bias towards favorable reviews from Vine members were assessed as well.

**First, reviews were extracted into a table in order to categorgize them into vine and non-vine member reviews in the final step:**

![Vine_df](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/Vine_df.png)

**Next, in order to filter out reviews that are likely to be helpful, customer id's that provided more than 20 reviews were gatherered into a dataframe:**

![total_votes](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/total_votes_helpful_df.png)

**Then, a percentage of helpful votes that are greater than 50% of the total votes are retrieved:**

![helpful_votes](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/helpful_votes.png)

**Finally, reviews written by vine members and non_vine members were gathered into their respective dataframes:**

* Vine reviews
![Vine_paid_df](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/Vine_paid_df.png)

-----------

* Non-vine reviews
![Non_Vine_unpaid_df](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/Non_vine_reviews_df.png)

## Results


**I. The total number of Vine reviews and non-Vine reviews are presented below:**
* Vine reviews

![Vine reviews](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/Vine_reviews.png)

*There are 94 vine reviews*

--------------

* Non-Vine reviews

![Non-Vine reviews](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/Non_vine_reviews.png)

*There are 40,471 non-vine reviews*

--------------
**II. The total number of Vine and Non-Vine 5-star reviews are presented below**
* Vine reviews

![Vine 5 star](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/5_star_reviews_vine.png)

*A total of 48 reviews were written by Vine members with 5 star ratings*

--------------

* Non-Vine reviews

![Non-Vine 5 star](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/5_star_reviews_non_vine.png)

*A total of 15,663 reviews were written by non-Vine members with 5 star ratings*

--------------
**III. The percentage Vine and Non-Vine 5-star reviews are presented below**
* Vine reviews

![Percentage Vine 5 star](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/5ded5354019f11afc0c31532c7255eb6ea33f440/Images/Perc_Vine_5star_reviews.png)

*51% of 5 star reviews were written by Vine members*

---------------

* Non-Vine reviews

![Percentage Non-Vine 5 star](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/Perc_Non_Vine_5star_reviews.png)

*39% of 5 star reviews were written by non-Vine members*

-----------------

## Summary
In summary, 51% of five star reviews were written by Vine members, compared to 38% written by non-Vine members. This difference indicates a postive bias towards positive reviews for video game products in the Vine program. A follow up analysis is recommended to look into the reviews of other products, specifically, technology products such as electronic equipments, within the 50 other datasets to determine whether such positive bias exists in other product reviews in order to get a larger assessment on whether such positive bias reviews exists within the Vine program as a whole.
