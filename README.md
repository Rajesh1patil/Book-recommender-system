# Book-recommender-system
 using collaborative book recommendation 


Problem statement

During the last few decades, with the rise of Youtube, Amazon, Netflix, and many other such web services, recommender systems have taken more and more place in our lives. From e-commerce (suggest to buyers articles that could interest them) to online advertisement (suggest to users the right contents, matching their preferences), recommender systems are today unavoidable in our daily online journeys. In a very general way, recommender systems are algorithms aimed at suggesting relevant items to users (items being movies to watch, text to read, products to buy, or anything else depending on industries). Recommender systems are really critical in some industries as they can generate a huge amount of income when they are efficient or also be a way to stand out significantly from competitors. The main objective is to create a book recommendation system for users.

Content

The Book-Crossing dataset comprises 3 files.

● Users

Contains the users. Note that user IDs (User-ID) have been anonymized and map to integers. Demographic data is provided (Location, Age) if available. Otherwise, these fields contain NULL values.

● Books

Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in the case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavors (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon website.

● Ratings

Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

Types of recommender sys

popularity based

content based

collaberative filtering

hybrid recommender

#Book Data

Data Description

Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in the case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavors (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon website.

#Users Data
Data description

Contains the users. Note that user IDs (User-ID) have been anonymized and map to integers. Demographic data is provided (Location, Age) if available. Otherwise, these fields contain NULL values.



#Popularity based Recommender System
Weighted average rating method
Using Weighted average for each Book’s Average Rating

W = Rv + Cm/(v + m)




Collaborative filtering
Collaborative filtering techniques create a model based on past user activity (items previously purchased, movies viewed and rated, etc.) as well as usage choices made by both current and past users. Then, this model is used to predict the ratings for items or items themselves that the user might be interested in.

where

W= Weighted Rating

R = Average of the Books rating

v = No of people who have rated the books(number of votes)

m = minimum no of votes to be listed

C = the mean rating across all the books





#Conclusion

The initial step,of our project was Data preprocessing of the three datasets-books_df,users_df and ratings_df,wherein we removed duplicates and imputed the missing values & invalid entries with appropriate values,corrected spellings.

Then,we performed Exploratory Data Analysis to find out the countries with maximum users,popular books,popular authors and popular publishing companies.We also analysed the rating distribution,age distribution of users and the popular books amongst various age groups .

Then,we used Popularity-based approach,Collaborative filtering approach to built different types of recommendation models.

*We evaluated the performance of Singular Value Decomposition based recommender and obtained a Global Recall@5 of 30 % and Recall@10 of 41%

Among top 20 Authors the highest number of books has been hold by Agatha Christie. Agatha Christie is leading at top with more than 600 counts, followed by William Shakespeare.

Harlequin has most number of books published, followed by Silhouette.

Number of Books published in yearly are between 1950 - 2005.

Most of the users are between 30-40 prefer more books and somewhat we can also view between 20-30.

As per ratings "Selected Poems" has been rated most followed by "Little Women". The countplot shows users have rated 0 the most, which means they haven't rated books at all.

The top 10 books recommendation as per ratings with top "The lovely Bones: A novel" with 707 book ratings. But this are not based on some recommendation system. They are top 10 books as per ratings.

As we perform by cosine similarity in recommendation system it gives 7.94 RMSE score and SVD improved score it to 1.63 RSME score by Singular Value Decomposition model (SVD).

The evaluation metrics for SVD is best RMSE score for all dataset (i.e users_data, ratings_data and books_data).

As model based approach was best to signify and at last we got top 10 recommended books and ratings respectively.

