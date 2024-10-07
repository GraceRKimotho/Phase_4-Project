# MOVIE RECOMMENDATION SYSTEM - HULU
![3bc2f36497f3f66074ba25515128e0d8](https://github.com/user-attachments/assets/a07857a2-3bff-4ace-b509-b20254ed3717)

## Introduction
In today’s highly competitive streaming landscape, personalized movie recommendations play a crucial role in user engagement and retention. Hulu, which holds 11% of the market share in the streaming industry, is looking to upgrade its current movie recommendation algorithm. The aim of this project is to develop a machine learning model that provides users with the top 5 movie recommendations based on their previous ratings of other movies.

Our audience for this project is the Hulu Technology Team, headed by the CTO of Hulu.This project will explore an enhanced algorithm to improve the quality of recommendations for Hulu subscribers.

## Data Understanding
The dataset used in this project was sourced from [Grouplens](https://grouplens.org/datasets/movielens/100k/), utilizing information from IMDb and TMDb. The data contains over 100,000 movie ratings provided by 610 different users for about 9,700 movies, collected over a time span from 1996 to 2018. Each user has reviewed at least 20 different movies.

While the full dataset consists of approximately 1.9 million ratings, this project focuses on a subset of 100,000 ratings due to time constraints.

## Overview
This project involves an exploratory data analysis (EDA) of a movie ratings dataset. The primary goal is to uncover insights into user preferences, genre popularity, and trends in movie ratings. The dataset includes over 765,000 movie entries, user ratings, and additional attributes such as movie genres and release years.

## Contents
- Data Description
- Exploratory Data Analysis
 - Univariate Analysis
 -Bivariate Analysis
- Results and Insights
- Conclusion
- Requirements
- Usage
- License

## Data Description
The dataset consists of the following key columns:

1.movieId: Unique identifier for each movie.

2.userId: Identifier for users who rated the movies.

3.rating: User rating for each movie (ranging from 0.5 to 5.0).

4.timestamp: The time when the rating was given.

5.release_year: The year the movie was released.

6.genres: Genre(s) associated with the movie.

7.tag: Tags assigned to the movie by users.

## Key Statistics
Total Entries: 765,271

Average Movie Rating: 3.99

Movies Released: 1921 - 2018

Most Frequent Genres: Drama, Thriller, Crime, Comedy, Action

## Exploratory Data Analysis
## Univariate Analysis
Summary Statistics: Basic statistics for key columns were computed, indicating a positive skew in movie ratings, with most ratings concentrated in the higher range (3-5).

### Distribution of Ratings: A histogram was generated to visualize the distribution of movie ratings.
![image](https://github.com/user-attachments/assets/2696a4a6-55c9-4313-b348-16de2e15461a)

The histogram shows that the majority of ratings are clustered between 3 and 5, with a peak around a rating of 4.

### Genre Distribution: A bar chart displays the most common movie genres.
![image](https://github.com/user-attachments/assets/7b1a590c-da31-4f40-ad94-93458819cf91)

This visualization reveals that Drama is the most prevalent genre, followed closely by Thriller and Crime.

### Top 20 Most Rated Movies: The most frequently rated films were identified and visualized.
![image](https://github.com/user-attachments/assets/81d8598a-881d-4ded-a8a9-dd45acec51d8)

Titles such as "Pulp Fiction" and "Fight Club" lead the list, indicating high user engagement.

### Top Tags: A bar chart shows the top 10 tags used in the dataset.
![image](https://github.com/user-attachments/assets/dfab050d-3cec-44e9-bc85-a1458e846e21)

"Thought-provoking" is the most frequently used tag, suggesting a preference for complex themes.

## Bivariate Analysis
- Ratings Per Movie: Movies were filtered to identify those with at least 100 ratings, allowing for analysis of popular films.

- Combined Metric for Popularity: A metric combining average ratings and the number of ratings was created to rank movies.

- Top Movies by Combined Metric: The top 10 movies based on the combined metric were visualized.
![image](https://github.com/user-attachments/assets/e34ae6ba-e2d4-4a48-ad5e-701dcc2c4e4a)

This chart highlights the most watched and highest-rated films, such as "The Shawshank Redemption."

## Most Popular Movies by Genre
A function allows users to input a genre and receive a list of the top-rated movies in that category.

## Results and Insights
The analysis indicates a preference for highly rated, critically acclaimed films, particularly in the Drama genre.
User engagement appears to favor blockbuster titles with higher ratings, such as "The Shawshank Redemption" and "The Godfather."
The genre distribution reveals that while there is a wide variety of movies, certain genres dominate user ratings.

## RECOMMENDATIONS
### Implement a Hybrid Recommendation System:

The hybrid model, which combines collaborative filtering (user-item interactions) and content-based filtering (movie features), shows promise in delivering more personalized and relevant recommendations. It can address the shortcomings of both methods, such as the cold start problem in collaborative filtering and the limited scope of content-based filtering.

### Incorporate User Feedback Loop:

Integrate a mechanism to collect explicit feedback (e.g., ratings) and implicit feedback (e.g., clicks, watch history) from users. This real-time data can continually refine the model, improving its accuracy and relevance.

### Periodically Retrain the Model:

User preferences and movie availability change over time. Regularly retraining the model on updated datasets will keep the recommendations current and align with shifting user interests.

### Include Diversity and Novelty:

While recommending popular titles is beneficial, incorporating lesser-known movies and genres can increase user engagement and broaden their viewing experience. Adjust model parameters to occasionally suggest niche content tailored to individual preferences.

### Enhance Genre-Specific Recommendations:

The analysis shows strong user interest in specific genres. Refine genre-based recommendation capabilities to allow users to explore top-rated and relevant titles within their favorite genres.

### Expand Evaluation Metrics:

In addition to RMSE and MAE, consider using precision, recall, and F1-score to evaluate the system's recommendation quality. User satisfaction surveys can also provide qualitative feedback for further improvements.

## CONCLUSIONS

### Effectiveness of the Hybrid Approach:

The hybrid recommendation system, combining both collaborative and content-based filtering, has demonstrated its capability to provide diverse and personalized movie suggestions. It effectively utilizes user ratings and movie features to align with individual preferences, offering robust recommendations even when limited user data is available.

### High User Engagement:

The analysis of popular movies and genres suggests that user interaction is significantly driven by specific genres (e.g., drama, thriller). The system capitalizes on this by using content-based filtering to surface genre-specific recommendations, further enhancing user satisfaction.

### Model Performance:

With an RMSE of 0.6434 and an MAE of 0.4992, the collaborative filtering model provides a reasonably accurate prediction of user preferences. Incorporating this into a hybrid system optimizes the balance between accuracy and diversity in recommendations.

### Future Enhancements:

While the current model performs well, future work should focus on dynamic updates through continuous retraining, integrating user feedback, and exploring additional filtering techniques (e.g., knowledge-based or context-aware recommendations) to cater to a broader range of user preferences and interactions.

Overall, the recommendation system lays a solid foundation for personalized movie suggestions, with room for ongoing refinement and enhancements to further engage users and improve their experience.








