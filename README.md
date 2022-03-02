# CIS544 Final Project

## Classifying Movies from their Revenue and Ratings

### Data

It has always been amongst my interests the acting world – because of this reason, I have chosen to do this analysis, since actors get paid according to how much the movie 

The data was extracted from Kaggle, so it is publicly available here. I chose the “IMDB Movie Dataset”, which has a bit less than 1000 rows of content and 16 variables. I did not use all of them – only the ones that were classified as integers or doubles, such as: IMDB Rating, Meta Score (score that was earned by the movie), Number of Votes, Gross (total revenue), Released Year and Run Time Min (duration of movie in minutes). Variables that were not considered for this study were the ones classified as factors, such as: Movie Title, Genre, Director, Stars, Classification, amongst others. 

### Procedure 
### Classifying data

Since we want to classify a movie from its revenue and ratings, we start by classifying the data by “Low”, “Mid” and “High” – we’ll be using the Meta_Score variable, which is the overall rating that was given to each movie. I have classified them as the following: Low<=50, Mid<=70 and High all the rest.

After classifying the data, we see that there are a total of 22 “Low” rated movies, 393 “Mid” rated movies, and 292 “High” rated movies.

After completing this, we proceed to perform the analysis with two different models. I have chosen KNN and Stepwise regression model. 

### KNN

For KNN I have chosen three different combinations of variables in order to see which one was more accurate. For the first one, I chose Gross (revenue) and Number of votes, and the accuracy was 47%. Since it was a low accuracy, I went for the second combination, which was the Released Year and Run Time of movie (in minutes) and its accuracy was of 59% - more than the previous one, but still low. So, I went for a third try, and did the combination of variables of IMDB rating and Number of votes and the accuracy rate was 51% - less than the previous one. 

### Stepwise Regression

I also performed Linear and Stepwise Regression and conducted its RMSE. For the linear regression the RMSE was 10.82. For the Stepwise Regression, it was the following: 
Stepwise Forward RMSE: 10.82127 
Stepwise Backward RMSE: 10.82127 
Stepwise Both RMSE: 10.92213 
So, very similar RMSEs. 


