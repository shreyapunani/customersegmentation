# Customer Segmentation- Data Analytics Project

Customer Segmentation has always been an important aspect of handling businesses related to services or goods. It is through customer segmentation that one realises if they are adopting the right strategies and are having happy consumers of their service. The following project utilises the Recency, Frequency and the Monetary Value approach (RFM) and the unsupervised learning model by clustering using K-Means. This repository contains two .ipynb for the two different methods used.

## Dataset
The dataset used here is the open-source [online retail](https://archive.ics.uci.edu/ml/datasets/Online+Retail) dataset by the UCI ML repository. For this project, the sales of Switzerland were considered because it is one of the countries in the world with the highest cost of living.

## Project Structure

1. Analysis using RFM Method
2. Analysis using K- Means Clustering ]
3. Visualizations- This folder contains all the charts and visual outputs generated during the analysis.

## RFM Analysis

The RFM Analysis involves the following parameters: R: Recency- Depicts the number of days passed since the last transaction. F: Frequency- Shows how frequent a customer comes and buys a product. M: Monetary Values- Depicts the total amount spent by that customer. For the RFM Analysis a RFM Table was constructed.

Post this, skewness was calculated

![skewness](https://github.com/user-attachments/assets/a8dad460-fa7f-4792-bbc6-62f4df6cd2c7)

The RFM data was divided into quantiles for analysing after which the RFM score was assigned to each of the customers. The RFM score determined the customer category. The different categories obtained were visualised using Plotly.


![Recency](https://github.com/user-attachments/assets/73933727-64c1-4da1-8dbd-da6481a137b7)
![Monetary](https://github.com/user-attachments/assets/f8fa7c8f-89f9-48de-9e8b-06657bd9832a)
![Frequency](https://github.com/user-attachments/assets/adbd52eb-0e8d-4acb-b0e6-b1971e9ab410)

After this, A square plot was plotted using squarify in order to analyse the segments with respect to a whole picture

![RMF Square Segments](https://github.com/user-attachments/assets/86498798-f420-4f6d-bc65-8e5fc2773aa6)

### Conclusion

The best customers spent a huge amount on online retail buying, were frequent and bought often. However a good amount of customers had less frequency and better marketing strategies like offer emails and discount vouchers should be adopted so that more customers are attracted.

## K-Means Clustering Method

First, Elbow Method is used to determine the number of optimal clusters.

![Elbow Method](https://github.com/user-attachments/assets/a524f7a6-8b33-4202-9e99-7078b3d06e47)


The graph shows that 3 number of clusters are ideal. This conclusion was derived because the graph takes a steep movement before 3 and becomes linear after it. Post this, the unsupervised K-means clustering model was fit to the dataset and then the results were visualized in a line plot by the seaborn library.
![Snake plot](https://github.com/user-attachments/assets/b9d2c197-5d37-4a5c-a57b-d516a1a3aa57)


A dot plot was plotted using Plotly in order to analyse the count in each cluster of customers.

![Cluster dot plot](https://github.com/user-attachments/assets/288c41a6-ba93-46f3-9d93-4aa06be35cdf)

### Conclusion

The Snake plot shows the monetary attribute and concludes that cluster 1 accounts to the best customers. Cluster 2 shows for the lost customers or churned customers. However, cluster 0 shows potential customers. They can be converted to the best customers by providing them with better incentives to shop.


This project helps identify the best strategies to better serve your customers.
