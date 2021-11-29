# Ukrainian coffee shops market analysis

In this project we'are going to perform analysis of coffee shops in Ukraine to find insights and present them to Marketing Team (non-technical).


## Dataset
Dataset has 200 rows and 9 columns (region, place name, type, rating, reviews, price and
services which propose to customers (Delivery, Dine in, Takeout). Part of information are missing.
Raw dataset available in `coffee_shops_dataset.csv`
## Libraries
The following libraries were used in the project: pandas, numpy, seaborn, matplotlib.pyplot, sklearn
## Steps
Three main steps can be differentiated in this project:
1. Data cleaning - checking, imputing and deleting data to prepare it for EDA and modeling
2. Exploratory Data Analysis (EDA) - visualization & looking for insights
3. Modeling - elbow method and k-means

## Model

The selected model was k-means with an 4 clusters selected by the elbow method.

![image](https://user-images.githubusercontent.com/64985339/143927942-bf235e9b-6270-4c05-8a63-ce0544c1e70b.png)

Clusters are covering data based on the rating and number of reviews.

![image](https://user-images.githubusercontent.com/64985339/143927988-24cbaf21-5aab-42dd-aa45-dd8f0e05c3bd.png)

| Cluster# | Description |
| ----------- | ----------- |
| Cluster 0 | high rating and low reviews |
| Cluster 1 | low raiting and low review |
| Cluster 2 | medium raiting and high reviews |
| Cluster 3 | medium raiting and low reviews |

## Conclusion
Cluster 2 was selected as the most promising because of the best performance compared to the others. 
Shops in Cluster 2 that provide all services are **21.2%** but..

![image](https://user-images.githubusercontent.com/64985339/143928207-b82b58be-abc3-4803-9afa-9efb39ef9f63.png)

..only dine-in & takeout options are possible is **36.4%** which are the highest result within all clusters.

![image](https://user-images.githubusercontent.com/64985339/143928247-7d3620ef-89c2-4b59-9c57-303195f6156f.png)

Places in cluster 2 are mostly located in Lviv and Kiev.

![image](https://user-images.githubusercontent.com/64985339/143928445-d7770600-354d-49c8-845f-3949eba4bdb0.png)

After a comprehensive analysis, it can be seen that coffee shops with at least two options (dine-in and takeout) in Lviv and Kiev have the highest probability of success.

Step by step analysis is available in `coffee_shops_CaseStudy.ipynb`.
Presentation for non-technical can be reviewed in `coffee_shops_presentation.pdf`

*This analysis was done as a final assignment for Data Scientist Professional certified by DataCamp which I successfully achieved.
