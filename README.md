# Movie_Recommender_system.
Aim :- It can recommend a movie that you are watched. this project is most useful in online platform like,You tube,instagram and job portals
it can takes previous or current data and it can be recoomend<br>
A Web Base user-item Movie Recommendation Engine using Collaborative Filtering By matrix factorizations algorithm and The recommendation based on the underlying idea that is if two persons both liked certian common movies,then the movies that one person has liked that the other person has not yet watched can be recommended to him.
<p>I've developed a similar application called "Movie_Recommender_system" which supports all language movies. But the only thing that differs from this application is that I've used the TMDB's recommendation engine in "Movie_Recommender_system". The recommendation part developed by me in this application doesn't support for multi-language movies as it consumes 200% of RAM (even after deploying it to Heroku) for generating Count Vectorizer matrix for all the 700,000+ movies in the TMDB. 

Link to "The Movie Cinema" application: [https://the-movie-cinema.herokuapp.com/](https://patilamit-movie-recommend-sys.herokuapp.com/)

Don't worry if the movie that you are looking for is not auto-suggested. Just type the movie name and click on "enter". You will be good to go eventhough if you made some typo errors.
</p>

![GitHub stars](https://img.shields.io/github/stars/rajaprerak/movie_recommender) 
[![Maintenance](https://img.shields.io/badge/maintained-yes-green.svg)](https://github.com/rajaprerak/movie_recommender/commits/master)
[![Website shields.io](https://img.shields.io/badge/website-up-yellow)](https://awesome-movie-recommender.herokuapp.com/)
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

### Website Preview
#### Home Page
![Screenshot (568)](https://user-images.githubusercontent.com/94529852/186221589-f7819811-9048-4e1e-a602-1b4a8f11eb28.png)

#### Detail Page
![Screenshot (569)](https://user-images.githubusercontent.com/94529852/186221650-17c26182-7a69-4570-ad53-d887830224b9.png)

----

## Installation 📦

>pip install -r requirements.txt



---
## Features 📋
* User can register and login.
* User can search through various movies and look through its details.
* User can give rating to the movies.
* User can add movie to their watch list.
* User can get movie recommendation (Recommendation algorithm (Collaborative Filtering) which suggests new movies based on the ratings given by user.)
---

## Algorithm
##### Collabortive Filtering (Recommender Algorithm)
* Collaborative filtering filters information by using the interactions and data collected by the system from other users. It's based on the idea that people who agreed in their evaluation of certain items are likely to agree again in the future.
* When we want to find a new movie to watch we'll often ask our friends for recommendations. Naturally, we have greater trust in the recommendations from friends who share tastes similar to our own.
* Collaborative-filtering systems focus on the relationship between users and items. The similarity of items is determined by the similarity of the ratings of those items by the users who have rated both items.
* There are two types of collaborative filtering
    * **User-based**, which measures the similarity between target users and other users.
    * **Item-based**, which measures the similarity between the items that target users rate or interact with and other items.
    > I have used **user based** collaborative filtering in this project.
     
     
  <br>
## Similarity Score : 

   How does it decide which item is most similar to the item user likes? Here come the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
## How Cosine Similarity works?
  Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
  
  ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)

  
More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

