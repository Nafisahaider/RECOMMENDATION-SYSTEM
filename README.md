# ANIME RECOMMENDATION-SYSTEM
This project implements a recommendation system for anime using collaborative filtering and matrix factorization techniques. The system is built using Python and leverages libraries such as pandas, numpy, scikit-learn, and surprise for data processing, model training, and evaluation.
Introduction
The goal of this project is to build a recommendation system that suggests anime to users based on their preferences. The system uses collaborative filtering and matrix factorization techniques to predict user ratings and recommend anime that users are likely to enjoy.

## Dataset
The dataset used in this project contains two main files:

anime.csv: Contains information about anime, such as anime_id, name, genre, type, episodes, rating, and members.

rating.csv: Contains user ratings for anime, with columns user_id, anime_id, and rating.

The dataset is loaded and preprocessed to handle missing values and undefined ratings.

## Installation
To run this project, you need to install the following Python libraries:

bash
Copy
pip install pandas numpy scikit-learn surprise matplotlib seaborn
Usage
Load the Dataset: The dataset is loaded from CSV files and preprocessed to remove missing values and undefined ratings.

Exploratory Data Analysis (EDA): The dataset is analyzed to understand the distribution of anime ratings.

Collaborative Filtering: A user-item matrix is created, and a k-Nearest Neighbors (kNN) model is used to find similar users.

Matrix Factorization: The Singular Value Decomposition (SVD) algorithm is used to predict user ratings.

Recommendation Function: A function is implemented to generate anime recommendations for a given user.

Show Recommendations: The system generates and displays top anime recommendations for a specific user.

## Methodology
Collaborative Filtering
Collaborative filtering is implemented using the NearestNeighbors algorithm from scikit-learn. The user-item matrix is created using the csr_matrix from scipy.sparse, and the kNN model is trained to find the most similar users.

## Matrix Factorization
Matrix factorization is performed using the SVD algorithm from the surprise library. The model is trained on the user-item rating data, and predictions are made for unseen anime.

## Recommendation Function
The recommendation function takes a user ID and the trained model as input, and returns the top anime recommendations based on predicted ratings.

## Results
The system successfully generates anime recommendations for a given user. For example, for user_id = 1, the top recommendations include popular anime such as "Kimi no Na wa." and "Steins;Gate Movie: Fuka Ryouiki no Déjà vu".

## Conclusion
This project demonstrates the implementation of a recommendation system using collaborative filtering and matrix factorization techniques. The system is capable of generating personalized anime recommendations based on user preferences. Future work could include exploring more advanced recommendation algorithms and incorporating additional features such as user demographics and anime metadata.
