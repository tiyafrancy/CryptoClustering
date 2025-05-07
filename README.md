# Module 19 Challenge    

In this challenge,  we will use our knowledge of Python and Unsupervised learning to predict if cryptocurrencies are affected by 24- hour or 7-day price changes.    
        
### Prepare the Data
     
Here, we use **.fit_transform** and **StandardScaler()** to normalize the data from the CSV file.    
Use **from sklearn.preprocessing import StandardScaler** line to import these dependencies.   

### Find the Best Value for k Using the Original Scaled DataFrame

Here, we found the best value of k using KMeans and elbow plot

<img width="728" alt="Screenshot 2025-05-07 at 12 50 57 PM" src="https://github.com/user-attachments/assets/00e367ca-f1d7-4224-8326-14b79046f2f6" />

### Cluster Cryptocurrencies with K-means Using the Original Scaled DataFrame

Here, we create clusters by using the best k value and create a scatter plot using hvplot

<img width="733" alt="Screenshot 2025-05-07 at 12 54 18 PM" src="https://github.com/user-attachments/assets/7f16c5ee-eb6d-4e82-a450-92516e6d356b" />

### Optimize Clusters with Principal Component Analysis

Here, we create a PCA model and use .fit_transform() to the original scaled dataframe

By, using the **explained_variance_ratio_**, we got that the total explained variance is 89.5%

### Find the Best Value for k Using the Scaled PCA DataFrame

Here, we again found the best k value on the PCA scaled dataframe and use elbow plot to show the result

<img width="737" alt="Screenshot 2025-05-07 at 12 59 27 PM" src="https://github.com/user-attachments/assets/b3ccd274-e712-489c-b505-b401d9d07e70" />

### Cluster Cryptocurrencies with K-means Using the Scaled PCA DataFrame

Here also, we create clusters by using the best k value from scaled PCA dataframe and create a scatter plot using hvplot

<img width="737" alt="Screenshot 2025-05-07 at 1 02 52 PM" src="https://github.com/user-attachments/assets/0ab920ef-9960-4ea4-8e4f-b4f2d60e3e3b" />

### Visualize and Compare the Results

In this section, you will visually analyze the cluster analysis results by contrasting the outcome with and without using the optimization techniques.

After visually analyzing the cluster analysis results, we can say that the second cluster, created using scaled PCA dataframe, shows the clusters which has only one data point separately and can be identified easily.

# Acknowledgement
          
I have done this challenge with the help of my Instructor, my classmate Dagim and some internet searches.



