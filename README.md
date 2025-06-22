
**Updated version of this application can be found at:** https://github.com/UmarBinAyaz/AJAX-Movie-Recommendation-System-with-Sentiment-Analysis-master

# Content-Based Movie Recommendation System with Sentiment Analysis

This project is a hybrid content-based movie recommender system that uses movie metadata and user review sentiment analysis to generate personalized movie suggestions. The system integrates TMDB API for real-time movie information, uses cosine similarity and Levenshtein distance for recommendations, and applies natural language processing (NLP) with a Multinomial Naive Bayes classifier to analyze user sentiments.
# ✨ Features

- Movie metadata fetched dynamically from TMDB API

- Asynchronous interaction using AJAX

- User review scraping from IMDb

- Sentiment classification using NLP

- Similar movie recommendations using cosine similarity and Levenshtein distance

- Frontend built with HTML, CSS, JS, and jQuery

- Backend implemented in Python using Flask

## The Movie Cinema

I've developed a similar application called "The Movie Cinema" which supports all language movies. But the only thing that differs from this application is that I've used the TMDB's recommendation engine in "The Movie Cinema". The recommendation part developed by me in this application doesn't support for multi-language movies as it consumes 200% of RAM (even after deploying it to Heroku) for generating Count Vectorizer matrix for all the 700,000+ movies in the TMDB. 


If you can't find the movie you're searching for through auto-suggestions while typing, there's no need to worry. Simply type the name of the movie and press "enter". Even if you make some typos, it should still work fine.

Source Code: https://github.com/UmarBinAyaz/AJAX-Movie-Recommendation-System-with-Sentiment-Analysis-master



## How to get the API key?

Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.


## Architecture

![Recommendation App](https://user-images.githubusercontent.com/36665975/168742738-5435cf76-1a42-4d87-94b4-999e5bfc48d3.png)


# Similarity Score:
How is the most similar item to the user's choice determined? This is where similarity scores come in.

A similarity score is a numerical value ranging from 0 to 1 that indicates how closely two items resemble each other. The higher the score, the more similar the items are. These scores are typically calculated by comparing the textual content of the items. One common method for computing this score is cosine similarity.

# How Does Cosine Similarity Work?
Cosine similarity is a technique used to measure the similarity between two text documents, regardless of their length. It does this by calculating the cosine of the angle between two vectors in a multi-dimensional space—each vector representing a document.

This method is especially useful because it focuses on the orientation rather than the magnitude of the vectors. So, even if two documents have different lengths, they can still be considered similar if they point in the same direction. The smaller the angle between the vectors, the higher the cosine similarity, indicating a stronger resemblance between the two items.

   ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)

### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)


