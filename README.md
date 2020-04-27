PROJECT STATUS: Ongoing

# Aim:
To build a showcase data science project for restaurant recommendation system, which will provide recommendation to users based on their preference.
This project has no commercial aspirations and is purely for academic purposes.
There are 2 major aspects of this project:

a) Getting the dataset- essentially restaurant IDs and user reviews

b) Building a recommendation system

This is an end-to-end data science project which showcases all aspects : data collection, data cleaning, data preprocessing, model construction and validation. 

Details are presented below:


## Data collection

The initial approach that was adopted was to self-collect the dataset. To build a user-item matrix for collaborative filtering, 30k+ restaurant business IDs were extracted from from Yelp API.
For user reviews, Yelp API returns 3 reviews per business ID. 
But we can only make 5000 API calls per day. Considering we have 30k+ business IDs X 3 reviews , it far exceeds 5000 API calls.
So the user reviews were retrieved in multiple chunks into dataframes. Specifically, the reviews dataframe consisted of:
1. business id
2. review id
3. user id
4. review text
5. rating
6. review time


This entire process can be found in this [Jupyter notebook](https://github.com/pritiM19/Restaurant-recommender/blob/master/scraping%20data%20from%20Yelp%20API.ipynb)

However, only 3 reviews per restaurant is very small dataset. 
So finally, I used the Yelp dataset on kaggle https://www.kaggle.com/yelp-dataset/yelp-dataset to build the recommender system.


## Data cleaning and exploration
....to be updated soon...
