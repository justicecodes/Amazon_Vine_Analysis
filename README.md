# Amazon_Vine_Analysis
## Overview:
Analysis on Amazon's vine review program to serve their client Sellby comparing reviews of their products to other similar products. The goal is to determine if a subscription to Vine is worth the cost for the company; i.e. if the Vine program makes a notable difference in review quality. Shoe reviews from Amazon were used for this analysis. Reviews of paid (Vine program) and unpaid customers are analyzed to determine if there is a difference.

#### Programming: 
* PySpark 
* AWS RDS 
* PostgreSQL
* Python Pandas Library (Jupyter Notebook)

## Results:
* 4,366,916 total shoe reviews analyzed
* Reviews with at least 20 total votes were used; at least 50% of those votes must have been marked as 'helpful votes'

#### Vine (paid) Reviews
* 22 total vine reviews
* 13 were 5 star reviews
* 59.1% of vine (paid) reviews were 5 star reviews
* 27.3% of reviews were 4 stars, ZERO (0.0%) were one star reviews

#### Unpaid Reviews
* 26,987 total non-Vine/unpaid reviews
* 14,475 were 5 star reviews
* 53.6% of unpaid reviews were 5 star reviews
* 15.0% of reviews were 4 stars, 14.5% were one star reviews

#### Average Review Rating
* 4.36 average rating of Vine (paid) reviews
* 3.86 average rating of unpaid reviews

## Summary: 
At a first glance, utilizing the Vine subscription seems to make a positive difference in review ratings for a company. The average rating for Vine reviews is .5 stars above the unpaid reviews left. 59% of Vine reviews were 5-Stars, while 54% of unpaid reviews were 5-Stars. Over 86% of Vine reviews are 4-5 stars; 68% of unpaid reviews were given as 4-5 stars.

However, when looking at other ratings, it is seen that 0 paid customers left a 1-Star review on the shoes from Amazon. However, 14.5% of unpaid reviewers left a 1-Star review. This discrepency could have been due to the filter that only 'helpful' reviews were analyzed (i.e. not many customers find 1-Star reviews 'helpful'). This observation is cause for concern that there may be bias or other motivation for the paid customers to leave positive reviews only, perhaps noting the product is inaccurately without fault. 

Overall, it is helpful from a client or company's perspective to subscribe to the Vine program to pay customers to test and review shoes on Amazon. 


#### Suggestions for further evaluation:
* Further analysis was done on other star ratings of the Vine reviews and unpaid reviews. Four star and one star ratings were observed, three and 2 star ratings could be ran to create a pie chart to visualize the percent given for each star rating.
* Calculate the average length in words of Vine reviews compared to non-paid reviews and total reviews - this could help determine if the vine reviews are longer or more detailed. Customers seem to get more benefit from more detailed reviews. 
* Percent of helpful reviews for paid Vine reviews vs. non-paid reviews - Did more people find the vine reviews helpful? (Are people swayed to vote a review at all or vote it as helpful if they see it is a paid review. Amazon adds disclaimers if the customer was part of a giveaway or paid program)
