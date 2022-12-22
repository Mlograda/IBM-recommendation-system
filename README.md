# IBM Recommendation system


## Project Overview

This project was designed to analyze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles that they might be interested in.

## Data Source

In this study, real data from the IBM Watson Studio platform were used. The datasets can be found in the data folder in this repository. 

## Project Content
### I. Exploratory Data Analysis
This space was used to explore the datasets, before diving into the details of the recommendation system in the later sections. There are some basic, required questions to be answered about the data I'm working with throughout the rest of the notebook. 
### II. Rank Based Recommendations
In this section I started building recommendations. First, I found the most popular articles simply based on the most interactions. Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

### III. User-User Based Collaborative Filtering
In order to build better recommendations for the users of IBM’s platform, I looked at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users. 

### IV. Content Based Recommendations
Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. Using NLTK,  I examined users that are similar in terms of the items' content they have interacted with. These items could then be recommended to similar users.

### V. Matrix Factorization
For the final step, I created a machine learning approach to building recommendations. Using the user-item interactions, I built out a matrix decomposition which helps me in predicting new articles an individual might interact with.



## Tools and Packages
---
```sh
# Packages
- Matplotlib
- Numpy
- Pandas
- Seaborn
- statsmodels
- Scikit-learn
- NLTK
- TfidfVectorizer
- cosine_similarity

```

## Acknowledgement

I would like to acknowledge and thank Udacity for giving me the chance to work on this project. I would also like to thanks IBM for providing the data.
