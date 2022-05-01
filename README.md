# Cryptocurrencies
# Introduction
In this challenge we create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. First, we process the data to make it ideal to fit the machine learning models. Since the target is unknown, we must use unsupervised learning. Finally, we do some data visualizations to have an easy understanding of the data.

## Preprocessing the Data for PCA 


First, we preprocess the dataset to perform PCA. 

<img width="831" alt="Screen Shot 2022-05-01 at 11 58 46 AM" src="https://user-images.githubusercontent.com/72629108/166160485-bf7a3857-b366-40b6-945f-06fc483154a0.png">

## Reducing Data Dimensions Using PCA 

We reduce the dimensions of the DataFrame to three principal components and place these dimensions in a new DataFrame.


<img width="776" alt="Screen Shot 2022-05-01 at 11 59 41 AM" src="https://user-images.githubusercontent.com/72629108/166160518-5bdec714-518d-4ce8-896c-9e1241db71bd.png">







## Clustering Cryptocurrencies Using K-means


Next step is Clustering Cryptocurrencies Using K-means. We create an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame. Then, we run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.

<img width="910" alt="Screen Shot 2022-05-01 at 12 00 29 PM" src="https://user-images.githubusercontent.com/72629108/166160544-79a199b0-0740-403e-934e-28d43316f733.png">

<img width="952" alt="Screen Shot 2022-05-01 at 12 03 22 PM" src="https://user-images.githubusercontent.com/72629108/166160625-a1eb0d73-82a5-4fa2-a57e-83d12c71f469.png">

<img width="989" alt="Screen Shot 2022-05-01 at 12 06 13 PM" src="https://user-images.githubusercontent.com/72629108/166160723-b16917e9-8952-48ef-9d3c-b7ff1990317c.png">


## Visualizing Cryptocurrencies Results

We create scatter plots with Plotly Express and hvplot, we visualize the distinct groups that correspond to the three principal components, then we create a table with all the currently tradable cryptocurrencies using the hvplot.table() function.

<img width="947" alt="Screen Shot 2022-05-01 at 12 05 00 PM" src="https://user-images.githubusercontent.com/72629108/166160691-312040fc-5cae-49a3-8095-400f4bb950e7.png">

<img width="938" alt="Screen Shot 2022-05-01 at 12 07 18 PM" src="https://user-images.githubusercontent.com/72629108/166160766-2686db1d-30b5-4209-b713-6f819fe99f50.png">

## Summary




