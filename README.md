# Amazon Vine Analysis

## Project Overview

The purpose of this analysis is to determine whether or not there is a bias inherent in Vine Amazon Reviews (expressed as a percentage of five star votes over total votes for Vine and non-Vine reviews).

For the sake of this analysis, we utilized Amazon Review data within the "PC" category. Utilizing PySpark, we create a summary table that tracks the aforementioned metrics by Vine and non-Vine Reviews to determine whether or not there is an inherent bias in the review process.

## Results

![alt text](https://github.com/lstanczyk90/Amazon_Vine_Analysis/blob/56e68ce73af0311edef9582c04c6a5a2dd818f76/Summary%20Statistics%20Table.png)

Please see the above DataFrame for the project statistics.

## Summary

Per our initial review, it would appear that there is no positivity bias for reviews in the Vine Program (please note that an analysis was only completed for the PC category, and the results for other categories may differ). Specifically, our analysis yielded that 44.11% of Vine Reviews were five-stars, while 46.45% of non-Vine reviews were five-stars. As such, it appears that Vine Reviewers do not leave more five-star reviews than non-Vine reviewers. 

### Suggestion for Additional Analysis

As noted above, our analysis was performed specifically for 5-star versus non-5-star reviews. However, to perform a more granular analysis, we should do the following:

- Create review buckets wherein we specify that reviews between 4-5 stars are positive, 3 stars are neutral, and less than 3 stars are negative. Then, we should compare summary statistics for these buckets to get more accurate representation.

- Additionally, a similar analysis should be performed for other sample categories, and the results should be compared across multiple categories. 