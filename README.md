# Grocery_Store_Customer_Segmentation
Performing customer segmention using RFM metrics and K-Means clustering algorithm

In this Project we will perform customer segmentation using RFM (Recency, Frequency, Monetary Value) metrics:

- Recency : How many days since last purchae
- Frequency : How many times a customer had transaction
- Monetary Value : Total revenue generated from this customer

Based on RFM metrics, we will segment the customer using K-Means Clustering algorithm.

## Raw Data
![image](https://github.com/AnthonyDjogan/Grocery_Store_Customer_Segmentation/assets/128353420/2ede114c-c090-4142-8182-ddd5eb5afc66)

## Transformed Data
![image](https://github.com/AnthonyDjogan/Grocery_Store_Customer_Segmentation/assets/128353420/74e9af28-ae52-4cae-a7c9-09f096de1284)

## Finding Best Number of Cluster
![image](https://github.com/AnthonyDjogan/Grocery_Store_Customer_Segmentation/assets/128353420/c1358381-06a2-42b6-ab39-83ea8a7ee041)
There is no clear elbow that can be seen from the plot, however if we examine the table, the difference in inertia values becomes less significant from 4 clusters onwards. Based on the silhouette score, the optimal number of clusters is 4, as it has a relatively high score above 0.5. A silhouette score above 0.5 usually indicates reasonably well-defined clusters, where there are significant differences in characteristics between clusters.

The final decision on the number of clusters should also take into account business context, not just based on the evaluation of inertia and silhouette score. It is crucial to strike a balance between granularity and practicality, ensuring that the chosen number of clusters aligns with the company's marketing strategies and objective.

For this project we will use 4 clusters.
## Result
![image](https://github.com/AnthonyDjogan/Grocery_Store_Customer_Segmentation/assets/128353420/71bd43f6-4274-443d-994c-b3ac96fa6c17)
![image](https://github.com/AnthonyDjogan/Grocery_Store_Customer_Segmentation/assets/128353420/286d012c-4114-467b-a266-b3eb816d5848)

## Insights:

**Cluster 4**: Recent purchases / High frequency / Highest monetary value
> Cluster 4 consists of the most valuable customers who have made recent and frequent purchases, contributing the most revenue for the business. The most bought product in this segment is non-food.

**Cluster 2**: Moderate purchases / Moderate frequency / Moderate monetary value
> Cluster 2 consists of customers who have made recent purchases and are moderately active compared to those in Cluster 4. They make purchases with a moderate frequency. The most bought product in this segment is non-food.

**Cluster 3**: Most recent purchases / Highest frequency / Low monetary value
> Cluster 3 comprises customers who make very recent and frequent purchases. Although their individual monetary value is lower compared to other clusters, they have a strong tendency to make purchases very recently. The most bought product in this segment is dairy.

**Cluster 1**: Highest recency / Lowest frequency / Lowest monetary value
> Cluster 1 consists of customers who have not made purchases recently and are less frequent spenders. Their individual monetary value is the lowest among the clusters, and they have the lowest frequency of buying. The most bought product in this segment is dairy.

Overall, the 4-cluster segmentation allows the company to better understand the diverse customer groups and formulate marketing strategies accordingly. By providing personalized experiences and targeted offers to each segment, the company can optimize customer retention and increase revenue gain from each customer group.
