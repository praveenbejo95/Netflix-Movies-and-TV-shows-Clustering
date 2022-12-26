# Netflix-Movies-and-TV-shows-Clustering


![image](https://user-images.githubusercontent.com/92503896/209543333-65471a82-7652-4cd0-92b8-0ecf7106d6b0.png)



## **Introduction:**

Netflix, Inc. is an American subscription streaming service and production
company. Launched on August 29, 1997, it offers a film and television series
library through distribution deals as well as its own productions. It’s is a very
popular streaming platform especially in countries like United States, India and
United Kingdom. This dataset consists of TV shows and movies available on
Netflix as of 2019. The dataset is collected from Flixable which is a third-party
Netflix search engine. It has 7787 entries and 12 attributes.

## **Problem Statement**

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

## **In this project, you are required to do**

1. Exploratory Data Analysis

2. Understanding what type content is available in different countries

3. Is Netflix has increasingly focusing on TV rather than movies in recent years.

4. Clustering similar content by matching text-based features

## **Attribute Information:**

show_id : Unique ID for every Movie / Tv Show

type : Identifier - A Movie or TV Show

title : Title of the Movie / Tv Show

director : Director of the Movie

cast : Actors involved in the movie / show

country : Country where the movie / show was produced

date_added : Date it was added on Netflix

release_year : Actual Releaseyear of the movie / show

rating : TV Rating of the movie / show

duration : Total Duration - in minutes or number of seasons

listed_in : Genere

description: The Summary description

## **Steps involved doing this project:-**

We featured engineered column for better intuition and followed data
preprocessing steps to make to data ready for model building. We converted
the data types of certain columns. We first began by handling the null
values. Maximum null values were present in the ‘director’ and ‘cast’ column,
as this are not important for model building, we dropped them.


For the text-based column we removed stop words and punctuations,
performed stemming and calculated TF-IDF. We performed this steps on
‘description’ and ‘listed_in’ column. As this is an unsupervised machine
learning problem, we used K-means to perform clustering.


We used elbow method to derive the most suitable number of clusters
giving us the acceptable error term with less computational cost. The
number of clusters for k-means clustering turned out to be 5. To measure
the goodness of clusters we used Silhouette score method. The score for 3
clusters are 0.34 which is good.


We used ‘length’ and ‘length_listed’ column for clustering purpose.
We did a thorough analysis of the data and extensive data preprocessing to
make the data ready for model deployment. After working on this dataset
we concluded that Netflix has been producing more movies than TV-shows

as almost 70% of the content on Netflix is of type movies and rest is TV-
shows. It’s most famous in United States and India. India is the only country

were content released is targeted towards teens. Movies and TV-shows
belonging to ‘TV-MA’ rating is highest on Netflix. It is for Mature audience
only.

## **Models Used**

      K means clustering
     
##**Metrics used**
      
      Silhouette coefficient or silhouette score
      
      Elbow Method
      

## **Conclusions:**

1. We've done null value treatment, feature engineering, and EDA since loading the dataset, and then we've completed some tasks that were assigned to us.

2. We have two types of content TV shows and Movies (30.86% contains TV shows and 69.14% contains Movies)

3. Netflix has increasingly focus on the movies than TV shows. It has been producing more movies than tv shows since after year 2014.

4. Netflix is most popular in United States. India lie at 2 position in popularity list.

5. In most of the countries the content available on netflix is mostly of movie type except in South Korea and Japan.

6. Clusttering was done using 'length' and 'length_listed' column.

7. Using elbow method and silhoutte score the best number of cluster turned out to be 3 with silhoutte score of 0.34 which is great indicating our clusters are homogeneous but heterogeneous to one another.
