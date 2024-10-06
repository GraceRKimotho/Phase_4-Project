# MOVIE RECOMMENDATION SYSTEM - HULU
![3bc2f36497f3f66074ba25515128e0d8](https://github.com/user-attachments/assets/a07857a2-3bff-4ace-b509-b20254ed3717)

## Introduction
In today’s highly competitive streaming landscape, personalized movie recommendations play a crucial role in user engagement and retention. Hulu, which holds 11% of the market share in the streaming industry, is looking to upgrade its current movie recommendation algorithm. The aim of this project is to develop a machine learning model that provides users with the top 5 movie recommendations based on their previous ratings of other movies.

Our audience for this project is the Hulu Technology Team, headed by the CTO of Hulu.This project will explore an enhanced algorithm to improve the quality of recommendations for Hulu subscribers.

## Data Understanding
The dataset used in this project was sourced from [Grouplens](https://grouplens.org/datasets/movielens/100k/), utilizing information from IMDb and TMDb. The data contains over 100,000 movie ratings provided by 610 different users for about 9,700 movies, collected over a time span from 1996 to 2018. Each user has reviewed at least 20 different movies.

While the full dataset consists of approximately 1.9 million ratings, this project focuses on a subset of 100,000 ratings due to time constraints.

### Key Features of the Dataset:
- User ID: A unique identifier for each user.
- Movie ID: A unique identifier for each movie.
- Ratings: A score from 0.5 to 5.0 given by a user for a movie.
- Timestamp: The time when the rating was provided.
- Movie Metadata: Information about the movies, such as title and genres.
This data is crucial for building a collaborative filtering model that can predict which movies a user is likely to rate highly based on the behavior of similar users.

## EDA
This project implements a hybrid movie recommendation system that combines collaborative filtering and content-based filtering techniques to provide personalized movie suggestions. The system utilizes user ratings and movie attributes to generate relevant recommendations, enhancing user experience in discovering new films.

### Features
1.Collaborative Filtering: Leverages user interactions and ratings to identify patterns and suggest movies that similar users enjoyed.

2.Content-Based Filtering: Analyzes movie attributes such as genres and titles to recommend similar films based on user-selected input.

3.Hybrid Approach: Merges both methodologies to improve recommendation accuracy and cater to diverse user preferences.

4.Temporal Recommendations: Considers the release year of movies for suggestions, enhancing relevance based on temporal proximity.

## MODELLING
- (Chosen Model, Evaluation, Deployment)
  
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








