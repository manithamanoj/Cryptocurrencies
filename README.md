# Cryptocurrencies
Introduction
In this challenge we create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. First, we process the data to make it ideal to fit the machine learning models. Since the target is unknown, we must use unsupervised learning. Finally, we do some data visualizations to have an easy understanding of the data.

Preprocessing the Data for PCA 


First, we preprocess the dataset to perform PCA. 

<img width="1032" alt="Screen Shot 2022-04-30 at 1 22 19 PM" src="https://user-images.githubusercontent.com/72629108/166160390-d6843561-4e64-440e-a7cc-4dad378a12b8.png">

Reducing Data Dimensions Using PCA 


We reduce the dimensions of the DataFrame to three principal components and place these dimensions in a new DataFrame.






Clustering Cryptocurrencies Using K-means



Next step is Clustering Cryptocurrencies Using K-means. We create an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame. Then, we run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.

Visualizing Cryptocurrencies Results

We create scatter plots with Plotly Express and hvplot, we visualize the distinct groups that correspond to the three principal components, then we create a table with all the currently tradable cryptocurrencies using the hvplot.table() function.






