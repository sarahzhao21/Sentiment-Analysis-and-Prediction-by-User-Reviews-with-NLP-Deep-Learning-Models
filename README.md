# Sentiment Analysis and Prediction by User Reviews with NLP Deep Learning Models.  

### Introduction
For this project, we would like to explore the relationship between yelp user reviews and yelp user ratings of restaurants. User rating is a good indicator of user attitudes towards local business. Inspired by the novel approaches that integrate NLP with deep learning, this project aims to train an algorithm that predicts the classes of user ratings with user reviews. This algorithm could be used to detect the user attitudes to restaurants from other crowdsourcing narratives (e.g. Tweets about restaurants) and can potentially expand the rating system of local restaurants.  

### Dataset
The datasets are retrieved from Yelp Dataset (https://www.yelp.com/dataset). It provides detailed information of businesses, users, reviews, etc. In our study, we will focus on the review and business datasets. We classified the reviews with the stars 4 or 5 as “good” and the reviews with 1 to 3 stars as “not-good.” In addition, since deep learning models require a substantial amount of computational power but the mode data could result in better outcomes, we need to find a subset of data with appropriate amounts of records. We finally chose data for the state of Pennsylvania for our project, which ranks the 6th for the count of reviews across the provided states.

### Exploration Data Analysis
We acquired a dataset of 344,253 records based on the user reviews of restaurants in Pennsylvania. The average rating of all selected reviews is 3.71 and the average length of reviews is 114 words. Most reviews give the restaurants five-star ratings while the least number of users give 2-star reviews. According to the graphs below, we found that positive reviews tend to be shorter than negative reviews with lower mean value of length and higher concentration of shorter reviews.
The Word Cloud shows that both types of reviews include keywords such as food and place. Positive reviews usually involve positive adjectives, however, negative reviews involve more verbs which indicates that negative reviews may more likely be given by users because of poor services.  

![count of rate of PA](https://github.com/sarahzhao21/SI-670-Maching-Learning-Project/blob/e3cca87bbed16b7294f06985631700e54c09f3a0/image/count%20of%20rate%20of%20PA.png). ![text length](https://github.com/sarahzhao21/SI-670-Maching-Learning-Project/blob/e3cca87bbed16b7294f06985631700e54c09f3a0/image/text%20length.png).  


### Machine Learning models
Three machine learning models were trained for this project. A baseline model with Naïve Bayes Classifier and two deep learning models. Our first deep learning model is based on Keras deep learning algorithm for text data classification, with two dense layers of the algorithm ‘relu’ and the last layer of the algorithm “sigmoid.” The second model is based on the advanced deep learning algorithms specific for text data analysis, which includes a Conv1D layer, a LSTM layer and three dropout layers in addition to the three regular layers.  We compared the accuracy and mean absolute error (MAE) of three models.The details are in the file of [SI670_project_Predicting_Yelp_Restaurant_User_Ratings_YC_MY_XZ.ipynb](https://github.com/sarahzhao21/SI-670-Maching-Learning-Project/blob/e3cca87bbed16b7294f06985631700e54c09f3a0/SI670_project_Predicting_Yelp_Restaurant_User_Ratings_YC_MY_XZ.ipynb) 

### Conclusion
With the trial of different combinations of deep learning algorithms and the adjustment of different hyper parameters, we found LSTM is the most effective model to predict the user rating classes. It can provide fairly accurate classification of the review data with a MAE of about 0.088 or less, which significantly outperforms the conventional multinomial naive Bayes classifier. It is obvious that the seemingly orderless user reviews actually contain hidden patterns that help us detect the attitudes of the reviewers.
![Poster_ Classifying Yelp User Rating with Yelp User Reviews](https://user-images.githubusercontent.com/54957469/119426199-c50e3d00-bcd6-11eb-9fce-ac7690411a9a.jpg)
