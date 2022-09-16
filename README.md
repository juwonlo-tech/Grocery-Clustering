# Grocery-Clustering

A grocery store would like to organize their products based on the co-purchase history of their customers.
They would also like to know the customer who bought the most items overall in their lifetime and who bought each product the most.
Another use case for this might be a recommender system for the store's web app.

## The Data

The data file contains to files, one containing the items sold and their respective IDs and the other containing the used_id and the comma-separated list of products purchased. together
The pre-processing of the data involves splitting and stacking the product ID column in the purchase history file to make it usable using pandas functions.
The new data frame is then merged with the data frame containing the product names.

## The Analysis and Results
Analysis shows that the user with ID 269335 has purchased the most products from the store.

<img width="794" alt="Screen Shot 2022-09-15 at 9 39 22 PM" src="https://user-images.githubusercontent.com/77176412/190545123-a795b0a3-ecac-463d-ac31-1a868f709451.png">

The result for the customers that bought the most of each product was also provided in the notebook.

Further computation was performed using one-hot encoding, principal component analysis (PCA), and K-Means clustering to create clusters of products that are regularly purchased together.
5 clusters were created and the products that made up each cluster was listed.

The output of the first 2 clusters can be seen in the image below.
<img width="794" alt="Screen Shot 2022-09-15 at 9 52 22 PM" src="https://user-images.githubusercontent.com/77176412/190546479-640a6f39-f431-4e41-8273-ac6ae93db595.png">
At first glance, it can be established that the first cluster contains fruits and the second contains vegetables. It is no surprise that these are commonly purchased together and can therefore be grouped together in the store.

The full script of the grocery clustering project can be found here: https://github.com/juwonlo-tech/Grocery-Clustering/blob/main/Grocery%20Clustering.ipynb
