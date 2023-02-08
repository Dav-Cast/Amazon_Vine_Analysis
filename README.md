# Amazon Vine Analysis

## Overview 
The main purpose of this analysis is to filter the reviews obtained from the Amazon Bucket as to verify and try to conclude if there is some kind of positive bias indulged over the paid Vine users. This will help get insights about the veracity of the reviews and the reviewers and overall it will help Amazon Vine to take measures as to make this service more reliable, trustworthy and honest for their users and clients.    

## Results
With the information in our control we had to filter out in different tables so as to have an order of the total reviews, 5 star reviews and finally get the percentage of 5 star for paid and unpaid Vine. ***The data was prepared before any filtering moves were made for this analysis, the data used was selected using only the one that have a 50% of helpful votes over total votes (as they are more reliable) and also two tables were obtained one for the paid user and the other for the unpaid as to make it easier to filter the information.***  

### Total Vine and non-Vine reviews
From the prepared data tables the next move was to only count the number of rows in each table as all the filtering was done before, separating both users using the column "vine" ('Y' for paid user and 'N' for unpaid). **So the total number of reviews for paid service is: 94 and for the unpaid service is: 40471.**

![Total_rev_Vine](https://user-images.githubusercontent.com/110573146/217635431-69431836-fd87-40ce-b5de-ef505c528f0a.png)

![Total_rev_notVine](https://user-images.githubusercontent.com/110573146/217635460-47f250f0-668e-424f-84ba-a0349105f371.png)

![Total_rev_dataframes](https://user-images.githubusercontent.com/110573146/217635627-1f15143b-91e5-4450-8c74-6e71a321f890.png)

### 5 star Vine and non-Vine reviews
For the 5 star reviews for both paid and unpaid it was necessary to create another two tables by filtering the data where the column "star_rating" was equal to 5, so a table was created from each. After getting these two new tables the same principle as the previous task was applied, all that is left is to count the number of rows in each table. **The total number of 5 star reviews for paid service is: 48 and for the unpaid service is: 15663.**

![5_star_rev](https://user-images.githubusercontent.com/110573146/217638110-fc3fc7b8-d3e9-4481-b0fe-75295b826ea5.png)

### Percentage of 5 star Vine and non-Vine reviews
For the calcuation of the percentage no new table was needed as all the information required was gathered in the previous tasks. The next step was to divide the number of 5 star reviews by the total number of reviews, this for both paid and unpaid and being careful as to not mix the numbers. **The % of 5 star reviews for paid service is: 51.06% and for the unpaid service is: 38.70%**

![Percentage_5_star](https://user-images.githubusercontent.com/110573146/217639370-1818f762-7cc8-4011-9658-951106f84fd7.png)

## Summary
Looking at the results it could be said that there is a possible positivity bias towars paid users in Amazon Vine, as there are way more unpaid reviews overall but ultimately the highest % of 5-star was for the paid (51%-paid and 39% unpaid). At least at first glance that is the conclusion one can come up with, but it would be a mistake to do it this way as more information is needed. We propose the following analysis as to come up with a much more rich information conclusion: 
- One option is to extend the same analysis we did, but for different datasets. In this analysis it was made for video-games, it could be done to toys and clothing as to get a more borad and wide view of the products reviews. Maybe they behave the same or maybe the same tendency is present.
- The second option is to instigate a little bit more in this dataset and review most of the products that were sent to the paid and unpaid users, maybe for a period of time the products were really better for the paid. So a analysis by periods of time would be good as to eliminate the probability of it being a seasonal thing and also a much more detailed study over the actual products would be good (although it would take more time) as to confirm the 5-star review.
