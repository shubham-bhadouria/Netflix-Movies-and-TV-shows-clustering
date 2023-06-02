# Netflix-Movies-and-TV-shows-clustering
![image](https://github.com/shubham-bhadouria/Netflix-Movies-and-TV-shows-clustering/assets/103518257/567dc546-df3c-44d2-9dc2-74002a09b8e9)

# Problem Statement
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

In this project, you are required to do:

- Exploratory Data Analysis
- Understanding what type content is available in different countries
- Is Netflix has increasingly focusing on TV rather than movies in recent years.
- Clustering similar content by matching text-based features

# Objectives:
- Conduct Exploratory Data Analysis.
- Try understanding what type content is available in different countries.
- Check if Netflix is increasingly focusing on TV rather than movies in recent years.
- Clustering similar content by matching text-based features.
# Methods used:
- Descriptive Statistics.
- Data Visualization.
- Machine Learning.
# Libraries utilized:
- NumPy and Pandas - For dataset cleaning and analysis.
- Matplotlib, Plotly and Seaborn - For Data Visualization.
- SkLearn and nltk - For machine learning and clustering.
# Dataset used:
This dataset consists of tv shows and movies available on Netflix as of 2019. It is collected from Flixable which is a third-party Netflix search engine.

# Attribute Information:
- show_id : Unique ID for every Movie / Tv Show
- type : Identifier - A Movie or TV Show
- title : Title of the Movie / Tv Show
- director : Director of the Movie
- cast : Actors involved in the movie / show
- country : Country where the movie / show was produced
- date_added : Date it was added on Netflix
- release_year : Actual Releaseyear of the movie / show
- rating : TV Rating of the movie / show
- duration : Total Duration - in minutes or number of seasons
- listed_in : Genere
- description: The Summary description

# Project Overview:
# Netflix Content Clustering and Recommender System

Netflix is a popular streaming service that offers a vast collection of award-winning TV shows, movies, anime, documentaries, and more, accessible on various internet-connected devices. The profitability of this business model relies on users making monthly payments to access the platform. However, customers have the freedom to cancel their subscriptions at any time. Hence, it is crucial for the company to keep users engaged and prevent them from losing interest. This is where recommendation systems play a pivotal role by providing valuable suggestions to users.

The aim of this project is to utilize K-means clustering and Agglomerative clustering techniques to form clusters based on Netflix content and subsequently build a simple recommender system.

In this project, I tackled a text clustering problem that involved classifying and grouping Netflix movies and shows into clusters based on their similarity. The dataset consisted of approximately 7787 records and 12 attributes. I began by addressing missing values in the dataset and performing exploratory data analysis (EDA). The analysis revealed that Netflix hosts more movies than TV shows and the number of shows and movies added to the platform is growing exponentially. Additionally, a majority of the shows were produced in the United States, and the content on Netflix primarily targets adults and teenagers.

After gaining valuable insights from the EDA, I proceeded to preprocess the text data by removing punctuation and stop words. The filtered data was then passed through a TF-IDF Vectorizer since we were conducting text-based clustering and the model required vectorized data to generate accurate predictions. The clustering was performed based on attributes such as director, cast, country, and description. The values in these attributes were tokenized, preprocessed, and vectorized using TF-IDF Vectorizer. This process resulted in a total of 20,000 attributes. To handle the curse of dimensionality, Principal Component Analysis (PCA) was employed. By selecting 5,000 components, over 95% of the variance was captured, thus limiting the number of components to 5,000.

Next, clusters were formed using the K-means clustering algorithm. The optimal number of clusters, which turned out to be 9, was determined through the elbow method and Silhouette score analysis. Additionally, clusters were created using the Agglomerative clustering algorithm, and the optimal number of clusters was found to be 11 by visualizing the dendrogram.

To provide personalized recommendations, a simple content-based recommender system was built using the similarity matrix obtained through cosine similarity. This recommender system generates 10 recommendations for users based on the type of show they have watched.

By leveraging clustering techniques and a content-based recommender system, this project contributes to enhancing the user experience on Netflix. The clusters help organize similar content, while the recommender system suggests personalized shows based on user preferences. This project demonstrates the effectiveness of machine learning in content analysis and recommendation systems, ultimately keeping users engaged and satisfied with their Netflix experience.

Finally, K–Means clustering and hierarchical clustering is utilized to form 10 distinct clusters with similar data points.

Using the data provided, we also implemented a simple recommender system that successfully generates Ten similar Movies or Tv-Shows for the given title.
