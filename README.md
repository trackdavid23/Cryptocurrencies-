# Project Overview
This project uses machine learning to identify which cryptocurrencies are on the trading market and to better understand how cryptocurrencies should be grouped to create classifications for developing an investment product. Unsupervised machine learning was chosen used since there is no known output for what I'm looking for. To group the cryptocurrencies, a clustering algorithm was also chosen to help determine whether or not I should be investing in this product.

Steps included in this project:

# Data preprocessing.
* This step included in-depth data cleaning, such as removing null values and removing cryptocurrencies without coins mined. In addition, the encoding method "get_dummies()" was used for the text features and StandardScaler() was used to standardize and transform the data.
* ![Screen Shot 2022-02-27 at 11 47 54 PM](https://user-images.githubusercontent.com/59430635/155925734-b5dc7d76-b302-4e61-9559-a193822c6dd9.png)

* Reducing data dimensions using PCA. In this step, a dataframe's dimensions was reduced to three principal components and a new dataframe was created.![Screen Shot 2022-02-27 at 11 49 09 PM](https://user-images.githubusercontent.com/59430635/155925823-4f3b8332-9059-40cd-9a82-fe7d7037079d.png)


* Clustering cryptocurrencies using K-means. During step, an elbow curve was created to find the best value for the clustering groups and a K-means algorithm was used to predict the K clusters for the cryptocurrencies’ data.![Screen Shot 2022-02-27 at 11 49 45 PM](https://user-images.githubusercontent.com/59430635/155925867-80ccca30-8952-4099-bd1d-73642abba4cf.png)
![Screen Shot 2022-02-27 at 11 49 59 PM](https://user-images.githubusercontent.com/59430635/155925884-b9807d0f-fb3d-4125-ada5-2f5dc672f04c.png)


* Visualizing results. In this final step, three types of figures were used: a 3D scatter plot to visualize the three PCAs, a hvplot.table to visualize all the current tradable cryptocurrencies, and a 2D scatter plot to visualize "Total Coins Mined" vs. "Total Coin Supply" by coin name and clusters.![Screen Shot 2022-02-27 at 11 50 27 PM](https://user-images.githubusercontent.com/59430635/155925925-d7c059d3-22b9-46e7-bef5-f257abbfe3ae.png)
