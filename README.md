# Capgemini_DataScience_TechChallenge_2021

Product Recommendation System (Capgemini Hackathon)
By: Sharvari Ballal

This project is about the product recommendation system of electronic and cloths products. 

Problem Statement:

Use Case:

Develop a product recommendation engine and detect the bias in recommendation if any. Two data sets are provided to you and you have to use them to build your solution. The solution should be able to provide recommendations based on the data and detect the bias if any.

Data Set:

Electronics.csv
ModCloth.csv

Deliverables :

Application/Solution source: should contain all the necessary source files. readme.txt: This should contain clear step-by-step instructions on how to build, deployment and usages of the Applications. Presentation.pptx: This should contain a description of what you have tried to build, what problem you are solving and why your Application/solution should be considered for the final round. (Sample Presentation.) Video showing the demo functionalities of the application (if applicable).

Technology/tools/libraries used:

-Python used for building this recommendation system, the Jupyter Notebook is used to write queries.
-Pandas and Numpy libraries used to perform EDA and feature engineering.
-Matplotlib, Seaborn libraries used to enhance the visualization of data. 
-scipy.sparse library is used for importing csr matrix
-sklearn.neighbors library is used for importing Nearest Neighbor

Program Files:

1. Product_Recommendation_System_Capgemini.ipynb
Please feel free to open this file on Jupyter or Google Colab to study the project or you can run this on this platform.
2. Electronic.csv
3. ModCloth.csv
4. Tech_Challenge_level_2_hackathon_template_2021.pptx
5. Readme.txt

Tour to project, lets see the step by step flow of model:

K Nearest Neighbor Algorithm

For this problem statment, I am using K Nearest Neighbor algorithm. KNN used as a good baseline for recommender system development. KNN first calculates the “distance” between the target product and every other product in the dataset. It ranks its distances and returns the top K nearest neighbor products as the most similar product recommendations. In which Cosine similarity will be applying, each and every product will be represented as vector and by using cosine similarity we can find the distance between two products by creating angle in between them and establishing relationship between them. Let's get started by very first step importing libraries!

Step 1 : Importing Libraries, loading data to form Dataframes & Preliminary Data Exploration
Step 2 : Data Cleaning (removing duplicate values and dealing with missing values)
Step 3 : Feature Engineering & Exploratory Data Analysis.
Step 4 : Data Visualization
Step 5 : Finding the total ratings count according to the item per User given
Step 6 : Define the popularity threshold from which we can select the most rated product
Step 7 : Implementing KNN Algorithm
Convert the table into 2D matrix and fill the missing values with zero, because we will calculate distance between rating vectors. Then transfer the ratings of the matrix dataframe into the scipy sparse matrix for more efficient calculation. Finding the Nearest Neighbor we used unsupervised algorithm with sklearn neighbor. The algorithm to compute the nearest neighbor is "brute" and metric is "cosine" so that the algorithm will calculate the cosine similarity between rating vector. After that we fit the model.





