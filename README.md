# Amazon_Vine_Analysis

## Overview

The overview of this project was to analyze Amazon reviews and do analysis on a portion of the reviews that are part of the Amazon Vine program. This program allows manufacturers and publishers to receive reviews of their products by way of members of their Vine program. The company provides products to their Vine customers who are then required to publish a review of the product. For this challenge, we were given the opportunity to select from approximately 50 different datasets of reviews. The dataset that we ended up selecting dealt with reviews relating to major appliances. We ended up using Pyspark to read in our data for the ETL process by way of using AWS. Then we loaded in our data into pgAdmin and then used PySpark to parse out the data we were looking for. After we completed our data analysis, we examined the results to see if there was any bias toward favorable reviews from the members of the Vine program.

## Results

### How many Vine reviews and non-Vine reviews were there?

<img width="386" alt="image" src="https://user-images.githubusercontent.com/110848660/211878928-e3175d3a-8035-4484-b81b-d59391ba1530.png">

<img width="386" alt="image" src="https://user-images.githubusercontent.com/110848660/211879003-02e696a2-bfb1-4d3e-91ee-c90e0d4c8453.png">

- We can see in the images above the number of Vine (paid) reviews and also the number of non-Vine (unpaid). The total number of Vine reviews was 248 while the number of non-Vine reviews was 96,653

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

<img width="461" alt="image" src="https://user-images.githubusercontent.com/110848660/211880647-12a763de-90aa-4eb0-9051-e61553d3d410.png">

<img width="430" alt="image" src="https://user-images.githubusercontent.com/110848660/211880856-398315a3-469d-4f98-9c52-90215f1f88c9.png">

- We can see in the images above the number of Vine (paid) reviews that were 5 stars was 112. We can also see that the total number of non-Vine (unpaid) reviews that were 5 stars was 49,592.

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

<img width="467" alt="image" src="https://user-images.githubusercontent.com/110848660/211881416-73b9c462-2cff-4d53-8404-62fb75c9acd0.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/110848660/211881461-6788c8ab-a3ef-4bde-91a7-1ec0aa877f8d.png">

- We can see in the images above the percentage of Vine (paid) reviews that were 5 stars was 45.16 %. We can also see that the percentage of non-Vine (unpaid) reviews that were 5 stars was 51.31 %.

## Summary
Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

We determined that there did not appear to be any bias when examining the 5-star reviews from the Vine program compared to the non-Vine 5-star reviews. We determined that by looking at our paid 5-star review percentage of 45.16 % and comparing that to the unpaid 5-star percentage of 51.31 %. The 5-star review percentage was higher for the non-Vine reviews so we believe there does not appear to be any strongly positive or negative bias.

Some additional analysis that we could do with the dataset to determine bias would be to look at other summary statistics. We could examine the same dataset any find the mean, median, and mode of scores among paid vs. unpaid reviewers. Just because the Vine reviewers did not give 5-star review ratings doesn't mean that they didn't show some sort of bias. It's possible that they showed bias but did so by grading reviews as mostly 4-star ratings instead of lower scores. 
