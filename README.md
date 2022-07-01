# Movie-Recommendations-System

There are basically **three** types of recommender systems:-

**Demographic Filtering** - They offer generalized recommendations to every user, based on movie popularity and/or genre. The System recommends the same movies to users with similar demographic features. Since each user is different , this approach is considered to be too simple. The basic idea behind this system is that movies that are more popular and critically acclaimed will have a higher probability of being liked by the average audience.

**Content Based Filtering** - They suggest similar items based on a particular item. This system uses item metadata, such as genre, director, description, actors, etc. for movies, to make these recommendations. The general idea behind these recommender systems is that if a person liked a particular item, he or she will also like an item that is similar to it.

**Collaborative Filtering** - This system matches persons with similar interests and provides recommendations based on this matching. Collaborative filters do not require item metadata like its content-based counterparts.

In this repository I have made three python kernels explaining and implementing the different types of movie recommender systems.

A webapp built using streamlit to display movie recommendation based on content based filtering using cosine similarity. 

- It gives recommendations based on movie content.
- One can give the movie title or director's name to get appropriate movie recommendations.


After preprocessing the datasets I decided to keep these columns in order to proceed further

| Column | Description |
| --- | --- |
| Movie ID | Unique ID for identification of movie and fetch appropriate poster for the same |
| Title| Title was used to get recommendations |
| Tags | Tags column was made using 'Overview','Cast','Genres','Keywords','Crew'|
| crew | Kept it to fetch recommendations based on Directors |

<p align='center'><img height='400' src = 'https://github.com/kartikdangi/Movie-Recommender-System/blob/main/src/Movie-Poster-Cliches-7.jpg'></p>
<br>
<h1 align='center'>Model deploy using Streamlit on Heroku Platform</h1>
[Link](https://movierecommendersystem12.herokuapp.com)
<br>
<p>In this project I have built a content based movie recommender system. The algorithm recommends products that are similar to the ones that a user has liked in the past. This similarity (generally cosine similarity) is computed from the data we have about the items as well as the user’s past preferences. </p>
<br>
<h2>What it does :</h2>
<p align='center'><img height='400' src = 'https://user-images.githubusercontent.com/31500911/145380710-1813c6e7-7635-47a6-b764-c4bd3315c9c1.png'></p>
<br>
<h2>Live Demo</h2>
<p align='center'><img height='400' src = 'https://user-images.githubusercontent.com/31500911/143416246-4bc98d07-12fa-404a-a98c-228eaaa6ef5c.gif'></p>
<br>
<h2>How it does : </h2>
<p>
Content Based Filtering - They suggest similar items based on a particular item. This system uses item metadata, such as genre, director, description, actors, etc. for movies, to make these recommendations. The general idea behind these recommender systems is that if a person liked a particular item, he or she will also like an item that is similar to it.
</p><br>
<h2>How to get the API key for images? : </h2>
<p>Create an account in https://www.themoviedb.org/, click on the API link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your API sidebar once your request is approved.</p>
<p align='center'><img src ='https://user-images.githubusercontent.com/31500911/143419982-2d726687-84d6-4616-8d09-833f732c92b2.png'></p>


<br>


<h2>Similarity Score : </h2>
<p>How does it decide which item is most similar to the item user likes? Here we use the similarity scores.
<br>
It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.</p>
<p align='center'><img src ='https://user-images.githubusercontent.com/31500911/143418326-9ed3e46a-5ddd-46dc-86fc-8b145101af52.png'></p>
<br>

<h2>How Cosine Similarity works? : </h2>
<p>Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.</p>
<p align='center'><img src ='https://user-images.githubusercontent.com/31500911/143417796-8602832b-aac9-4f4f-b930-b753dc050981.png'></p>
<br>
<h2>Sources of the datasets : </h2>
<p>I have used the TMDB 5000 movies dataset to build the model</p>
<p>You can collect dataset from https://www.kaggle.com/tmdb/tmdb-movie-metadata</p>

### List of other dataset

* MovieLens - Movie Recommendation Data Sets [link](https://grouplens.org/datasets/movielens/)
* Netflix Prize Dataset [link](http://academictorrents.com/details/9b13183dc4d60676b773c9e2cd6de5e5542cee9a)
* Yahoo! - Movie, Music, and Images Ratings Data Sets [link](https://webscope.sandbox.yahoo.com/catalog.php?datatype=r)
* Cornell University - Movie-review data for use in sentiment-analysis experiments [link](http://www.cs.cornell.edu/people/pabo/movie-review-data/)
* MovieTweetings - [link](https://github.com/sidooms/MovieTweetings)
