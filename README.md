## Cryptocurrencies

## Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features.
This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.
We use the following methods for the analysis:

- preprocessing the database,
- Reducing the data dimension using Principal Component Analysis,
- Clustering cryptocurrencies using K-Means,
- Visualizing classification results with 2D and 3D scatter plots.

## Resources
Data Source: crypto_data.csv, CryptoCompare
Software: Python 3.7.7, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results
Following the preprocessing and cleaning phase we have a total of 532 tradable cryptocurrencies.


### Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know what would be the output of the analysis so we are using unsupervised machine learning to identify clusters of the cryptocurrencies.
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.

<img width="532" alt="image" src="https://user-images.githubusercontent.com/104597335/188495987-c4391ccf-969a-44ea-90ce-14b248ad56e3.png">


The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

### Visualizing Cryptocurrencies Results
#### 3D-Scatter plot with clusters

<img width="587" alt="image" src="https://user-images.githubusercontent.com/104597335/188496038-a44f709f-4e5f-4922-bb16-4362c4cc17b0.png">



This 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.

#### 2D-Scatter plot with clusters

<img width="577" alt="image" src="https://user-images.githubusercontent.com/104597335/188496076-840ce96d-cd6d-472e-bb08-63db5ec01239.png">



This 2-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to two principal components.

Both these scatter plots show the distribution and the four clusters of cryptocurrencies.
We can identify the outliers like the unique cryptocurrency in the class #2.


#### Tradable Cryptocurrencies Table

<img width="573" alt="image" src="https://user-images.githubusercontent.com/104597335/188496103-0be68960-8498-41f3-bf75-752bb8555243.png">



Most of the cryptocurrencies are part of class #0 and #1.
The snapshot above shows that BitTorrent is the only cryptocurrency in class #2.

#### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply

<img width="561" alt="image" src="https://user-images.githubusercontent.com/104597335/188496129-f1725cea-263f-4704-8509-6ef89a4d2ea2.png">



Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Then using the PCA algorithm is the right method for better visualizations.

## Summary
We have identified the classification of 532 cryptocurrencies based on similarities of their features.
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.
