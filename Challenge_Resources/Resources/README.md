# Detailed Instructions From Your Instructor Team

The objective of this challenge is for you to preprocess the data set using Pandas, reduce the dimensions to three principal components using PCA, predict clusters using the K-means algorithm, create an Elbow curve to find the best value for K,create a 3D-scatter plot using Plotly Express, create a 2D scatter plot using Holoviews, and a create table with tradable cryptocurrencies for your results.

## Deliverable 1: Preprocessing the Data for PCA 

For the first deliverable, we are asking you to preprocess the cryptocurrency data set in order to perform PCA in Deliverable 2. 

You should not find the tasks to complete this deliverable difficult, because you should be familiar with cleaning data. After you clean the data you'll need to use the StandardScaler library to standardize features. 

We have provided [starter code](./Resources/crypto_clustering_starter_code.ipynb) to help you get started. You'll need to add your code to the empty input cells to get the output shown.

## Deliverable 2: Reducing Data Dimensions Using PCA

For the second deliverable, you will apply the PCA algorithm to reduce the dimensions of the `X` DataFrame to three principal components and place these dimensions in a new DataFrame named `pcs_df`.

You should not find the tasks to complete this deliverable to be difficult since you have been introduced in Lesson 18.5.2.  

In the [starter code](./Resources/crypto_clustering_starter_code.ipynb) we have provided the empty input cells where you'll need to add your code to get the output shown. 

All you'll need to do is reduce the dimensions to three principal components and add those three dimensions to a new DataFrame. 

## Deliverable 3: Clustering Cryptocurrencies Using K-means

For the third deliverable, you will create an elbow curve using `hvPlot` to find the best value for K from the `pcs_df` DataFrame created in Deliverable 2. Then, you’ll run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.

You should not find the tasks to complete this deliverable to be difficult since you have been introduced in Lessons 18.3.2, 18.4.2, and 18.5.2. 

Like Deliverables 1 and 2, we have provided instructions in the [starter code](./Resources/crypto_clustering_starter_code.ipynb) to assist you with this deliverable. In addition, there is a link to KMeans documentation.

* First, you'll need to create an elbow curve using `hvPlot` to find the best value for K.

* Next, you'll run the K-means algorithm on the the `pcs_df` DataFrame to make predictions of the K clusters for the cryptocurrencies’ data.

* Then, you'll need to create a new DataFrame, `clustered_df`, by concatenating the `crypto_df` and `pcs_df` DataFrames on the same columns. Add then `CoinName` and `Class` columns to the `clustered_df` DataFrame.

## Deliverable 4: Visualizing Cryptocurrencies Results

For the last deliverable, you will visualize your results by creating scatter plots with Plotly Express and `hvplot` and create a table with all the current tradable cryptocurrencies using the `hvplot.table()` function.

you may find the tasks to complete this deliverable to slightly difficult. Some steps have been covered in Lessons 18.3.2 and 18.4.2.  However, we have provide [starter code](./Resources/crypto_clustering_starter_code.ipynb), where you will need to add your code to the empty input cells to get the output shown.

We have also provided links to documentation to do the following tasks:
* Add additional parameters to a Plotly Express 3D scatter plot.
* Create a table using the `hvplot.table()` function.
* Use the `MinMaxScaler().fit_transform` method to scale the "TotalCoinSupply" and "TotalCoinsMined" columns.
* And, customize the `hvplot` scatter plot. 

## Submission

Make sure you upload the following to your Cryptocurrencies GitHub repository:

1. your `crypto_clustering.ipynb` file.
2. A README.md that includes the purpose of the repository and short description of what was accomplished. Although there is no graded written analysis for this challenge, it is encouraged and good practice to add a brief description of your project.

## Grading Rubric

The [Unsupervised Learning Grading Rubric](./Resources/Module_18_Challenge_Grading_Rubric.pdf) is provided for you to use when grading you' submissions.
