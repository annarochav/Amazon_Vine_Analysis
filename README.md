# :shopping_cart: Amazon_Vine_Analysis :shopping_cart:

Challenge Week16 Data Analysis BootCamp using AWS, PySpark and Postgres.


<img src="https://github.com/annarochav/Amazon_Vine_Analysis/blob/main/Resources/what-is-amazon-vine-program-adlucent.jpg" width="1000" height="" />

## ⚡Overview of the analysis:

This project consists of determine if there are any biases between Vine members and non-Vine member's Beauty products reviews. A Vine program means that some companies receive products and are required to make a review, these reviews must be objective and free from bias to be valuable data. 

For this analysis, an ETL process was used to extract data from an AWS RDS, transformed it with PySpark and loaded to a Postgres Database.

## ⚡Results: 

**1. How many Vine reviews and non-Vine reviews were there?**

 + The dataset that was extracted from AWS had 5,115,452 Beauty reviews, so only reviews with 20 or more votes and 50% helpful criteria where considered for the analysis leaving 74,760 reviews. 

 + Of the 74,760 reviews, 647 were from Vine members (paid) and 74,113 were from non-Vine members (unpaid).
 
 <img src="https://github.com/annarochav/Amazon_Vine_Analysis/blob/main/Resources/1_results.png" width="700" height="" />

**2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**

 + There was a total of 43,446 5-star reviews. Out of that total, 229 were 5-star Vine reviews, and 43,217 were 5-star non-Vine reviews.
 
 <img src="https://github.com/annarochav/Amazon_Vine_Analysis/blob/main/Resources/2_results.png" width="550" height="" />
 
**3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**

 + The percentage of total 5-star Vine reviews of total Vine reviews was 35.39%.
 + The percentage of total 5-star non-Vine reviews of total non-Vine reviews was 58.31%
 
  <img src="https://github.com/annarochav/Amazon_Vine_Analysis/blob/main/Resources/5_results.png" width="350" height="" />

## ⚡Summary: 

Since 58.31% of the 5-star reviews come from non-paid customers, **the reviews from the Vine program members seem to be objective and without bias**, 35.39% was the result. Additional analysis must be made to make better conclusions, for example, we can filter by product category or brand. Also we can compare 3 and 4 stars and see if there is any difference.

