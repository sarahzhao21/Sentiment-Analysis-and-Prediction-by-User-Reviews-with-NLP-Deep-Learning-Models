# Sentiment Analysis and Prediction by User Reviews with NLP Deep Learning Models.  

### Introduction
For this project, we would like to explore the relationship between yelp user reviews and yelp user ratings of restaurants. User rating is a good indicator of user attitudes towards local business. Inspired by the novel approaches that integrate NLP with deep learning, this project aims to train an algorithm that predicts the classes of user ratings with user reviews. This algorithm could be used to detect the user attitudes to restaurants from other crowdsourcing narratives (e.g. Tweets about restaurants) and can potentially expand the rating system of local restaurants.  

### Dataset
The datasets are retrieved from Yelp Dataset (https://www.yelp.com/dataset). It provides detailed information of businesses, users, reviews, etc. In our study, we will focus on the review and business datasets. We classified the reviews with the stars 4 or 5 as “good” and the reviews with 1 to 3 stars as “not-good.” In addition, since deep learning models require a substantial amount of computational power but the mode data could result in better outcomes, we need to find a subset of data with appropriate amounts of records. We finally chose data for the state of Pennsylvania for our project, which ranks the 6th for the count of reviews across the provided states.

### Exploration Data Analysis


### Machine Learning models
Three machine learning models were trained for this project. A baseline model with Naïve Bayes Classifier and two deep learning models. Our first deep learning model is based on a regular deep learning algorithm for text data classification, with two dense layers of the algorithm ‘relu’ and the last layer of the algorithm “sigmoid.” The second model is based on the advanced deep learning algorithms specific for text data analysis, which includes a Conv1D layer, a LSTM layer and three dropout layers in addition to the three regular layers.  We compared the accuracy and mean absolute error (MAE) of three models. 
![Poster_ Classifying Yelp User Rating with Yelp User Reviews](https://user-images.githubusercontent.com/54957469/119426199-c50e3d00-bcd6-11eb-9fce-ac7690411a9a.jpg)
