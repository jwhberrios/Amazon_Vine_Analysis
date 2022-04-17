# Amazon_Vine_Analysis
Big Data Analysis using PySpark and the ETL process to anaylze large data sets of amazon purchase reviews. AWS database and PostgreSQL tables using PgAdmin were used to analyse the video game product dataset. 

### Overview
The purpose of this analysis is to assess Amazon product reviews written by members of the paid Amazon Vine program, specifically, video game products. Any bias towards favorable reviews from Vine members were assessed as well.

### Results
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

*A total of 15,663 reviews were written by Non-Vine members with 5 star ratings*

--------------
**III. The percentage Vine and Non-Vine 5-star reviews are presented below**
* Vine reviews

![Percentage Vine 5 star](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/5ded5354019f11afc0c31532c7255eb6ea33f440/Images/Perc_Vine_5star_reviews.png)

*51% of 5 star reviews were written by Vine members*

---------------

* Non-Vine reviews

![Percentage Non-Vine 5 star](https://github.com/jwhberrios/Amazon_Vine_Analysis/blob/main/Images/Perc_Non_Vine_5star_reviews.png)

*39% of 5 star reviews were written by Non-Vine members*

-----------------

### Summary
In summary, 51% of five star reviews were written by Vine members, compared to 38% written by non-Vine members. This difference indicates a postive bias towards positive reviews for video game products in the Vine program. A follow up analysis is recommended to look into the reviews of other products, specifically, technology products such as electronic equipments, within the 50 datasets to determine whether such positive bias exists in other product reviews in order to get a larger perception on whether such positive bias reviews exists within the Vine program as a whole.
