# Netflix-Movies-And-TV-Shows-Clustering

![venti-views-lI7dlA5VBp8-unsplash](https://github.com/KashmiraKor/Netflix-Movies-And-TV-Shows-Clustering/assets/80064697/a693a987-f4c6-42cf-8082-36c019ace26e)

## Project Summary -
The project aims to conduct an in-depth exploratory data analysis of Netflix content, focusing on understanding content distribution across countries, trends in TV shows versus movies, integration with external datasets for enrichment, clustering similar content based on text-based features, and analyzing user engagement metrics.

By leveraging the dataset alongside external sources like IMDB ratings and Rotten Tomatoes, we can uncover valuable insights into Netflix's content landscape and audience preferences. These insights are crucial for Netflix to refine its content strategy, optimize content acquisition, and enhance user satisfaction and engagement.

Through this project, we aim to provide actionable recommendations for Netflix to strengthen its content portfolio, cater to diverse audience preferences, and maintain its position as a leading streaming service in the ever-evolving entertainment industry.

## Problem Statement - 
As the streaming industry continues to evolve, Netflix, a prominent player in the market, faces the challenge of effectively managing its vast content library to meet the diverse preferences of its global audience. Despite the availability of extensive data on Netflix's content, including TV shows and movies, sourced from platforms like Flixable, there remains a need to extract actionable insights to inform strategic content decisions. Specifically, the project seeks to understand content distribution across different countries, evaluate if Netflix has been shifting its focus from movies to TV shows in recent years, cluster similar content based on text-based features, and analyze user engagement metrics. By doing so, the project aims to provide valuable insights and recommendations to Netflix for refining its content strategy, optimizing content acquisition, and enhancing user satisfaction and engagement on its platform.

## Methods used -
- Descriptive Statistics.
- Data Visualization.
- Machine Learning.
  
## Libraries utilized -
- NumPy and Pandas - For dataset cleaning and analysis.
- Matplotlib, Plotly and Seaborn - For Data Visualization.
- SkLearn and nltk - For machine learning and clustering.

## Variable Information -
- show_id: Unique identifier for each show or movie in the dataset.
- type: Indicates whether the entry is a TV show or a movie.
- title: The title of the TV show or movie.
- director: The director(s) of the TV show or movie.
- cast: The main cast members of the TV show or movie.
- country: The country or countries where the TV show or movie was produced.
- date_added: The date when the TV show or movie was added to Netflix.
- release_year: The year when the TV show or movie was released.
- rating: The age rating or maturity rating of the TV show or movie.
- duration: The duration (in minutes or seasons) of the TV show or movie.
- listed_in: The categories or genres the TV show or movie belongs to.
- description: A brief description or summary of the TV show or movies.

## Conclusion

In our project, we embarked on a comprehensive exploration of a dataset comprising 7787 records and 12 attributes from Netflix, with a primary focus on addressing missing values and conducting insightful exploratory data analysis (EDA).

### Key Insights:
Our analysis revealed intriguing trends within the dataset. Notably, we observed that Netflix boasts a vast collection of movies compared to TV shows, with a notable surge in the acquisition of shows originating from the United States.

### Feature Selection and Transformation:
To effectively cluster the shows, we strategically selected six pivotal attributes: director, cast, country, genre, rating, and description, all of which were categorical variables. We transformed these attributes into a 9000-feature TF-IDF vectorization. To mitigate the curse of dimensionality, we employed Principal Component Analysis (PCA), reducing the components to 2500 while retaining over 80% of the variance.

### Clustering Analysis:
Utilizing K-Means and Agglomerative clustering algorithms, we endeavored to group the shows based on their inherent similarities. The elbow method in K-Means analysis confirmed the optimal number of clusters to be 6. However, Silhouette score analysis suggested 5 clusters. In Agglomerative clustering, the optimal number of clusters was again determined to be 6, which we vividly visualized using a dendrogram.

### Recommender System Development:
Building upon our clustering efforts, we developed a sophisticated content-based recommender system. Leveraging the similarity matrix derived through cosine similarity, our system offers personalized recommendations tailored to the user's viewing history. By analyzing the types of shows the user has watched, it furnishes ten top-notch suggestions, empowering users to delve into captivating content aligned with their preferences.


