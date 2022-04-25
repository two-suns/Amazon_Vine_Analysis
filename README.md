# Amazon Vine Analysis
## Overview
Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

## Results
  - How many Vine reviews and non-Vine reviews were there?
    - ![paid_tot](https://user-images.githubusercontent.com/59906657/165003935-00f5e85c-c994-4dac-819f-87f8590d74f1.PNG)
      - 94 total Vine reviews
    - ![unpaid_tot](https://user-images.githubusercontent.com/59906657/165003973-42926f92-14a9-4657-9992-f87ac5db0058.PNG)
      - 40471 total non-Vine reviews

  - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
    - ![paid_five_star](https://user-images.githubusercontent.com/59906657/165004049-ee03f464-c0b0-41d2-b175-31088b067b68.PNG)
      - 48 Vine reviews were 5 star.
    - ![unpaid_five_star](https://user-images.githubusercontent.com/59906657/165004075-40a78a7f-2887-4ee0-afea-bc3ebb4d2281.PNG)
      - 15663 non-Vine reviews were 5 star.

  - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
    - ![prcnt_paid](https://user-images.githubusercontent.com/59906657/165004141-dceb3d39-bf06-4e06-9d3a-bfb9fd9e82b1.PNG)
      - 51.06% of Vine reviews were 5 stars.
    - ![prcnt_unpaid](https://user-images.githubusercontent.com/59906657/165004181-cfbad5f4-0230-4116-a23c-d9b5f912c304.PNG)
      - 38.7% of non-Vine reviews were 5 stars.

## Summary
I believe a sufficient amount of reviews, over 40,000, were analyzed which would limit positivity bias.  The parameters were not overestimated. However, the paid reviews were a much smaller subset.  The paid reviewers were slightly more satisfied with the video games with 51.06% giving 5 star reviews.  An additional analysis that could be conducted would be to use the verified purchase column. This could be used to determine if the results could be skewed due to ratings boosting by people who have not actually purchased the game.   
