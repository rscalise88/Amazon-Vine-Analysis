# Amazon Vine Analysis

## Project Overview
Through the Amazon Vine service, manufacturers can receive products for their products through third-party companies who provide these products to customers, who are then required to provide a review of the product they received.  Amazone review information is freely available as datasets, broken down by product type.  Here, I review the Electronics dataset and attempt to determine is the paid reviews have a positive bias towards 5-star reviews.

## Resources
AWS RDS, PySpark, ETL, pgAdmin, SQL, Pandas.

## Results
Vine Paid Reviews:

![1](https://github.com/rscalise88/Amazon-Vine-Analysis/blob/main/images/2.PNG)
  - There are 1080 paid Vine reviews.
  - 454 of the Vine reviews are 5-star reviews, 42% of the total


Unpaid Reviews:

![2](https://github.com/rscalise88/Amazon-Vine-Analysis/blob/main/images/1.PNG)
  - There are 49673 unpaid/normal reviews from the general public
  - 23043 of these reviews are 5-star reviews, 46% of the total.

## Summary
Based on the data found in the analysis, it does not appear that there is a correlation between paid reviews and positivity.  To the contrary, a slightly higher percentage of the reviews from the general public were positive compared to the paid vine reviews.

For further analysis, it would be wise to not just look at the 5-star reviews as a function of total reviews, but also the 1 or 2 star reviews as well.  Limiting our definition of "positive" to 5 instead of 4-5, and ignoring whether or not paid reviewrs have a tendency to *not* leave 1-2 star reviews would provide us with a better picture of what kind of influence being paid to review a product may or may not have on the bias of the reviewer.
