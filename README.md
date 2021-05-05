## MOVIE RECOMMENDER SYSTEM - USING MOVIELENS DATA

#### About
Personalized recommendations are of key importance when it comes to increasing business value and sales of products and customer retention and satisfaction. Companies generate higher revenues and save resources, by simply understanding individual customer behaviors. In recent times, a large portion of the information we see online comes from recommendations catered to us based on content or products we have previously liked or invested in. Grouping similar users or items can allow for vast exposure of products to multiple users. It also solves the issue of the cold-start problem for new users. 

Recommender systems are mainly of 2 types – Content-based Filtering and Collaborative Filtering (Memory-based and Model-based). Using both Implicit and Explicit ratings, companies can recommend relevant content to their users. This paper aims to describe a movie recommender system that utilizes explicit ratings and movie genres to make personalized recommendations. Machine Learning methods including Term Frequency and Inverse Document Frequency (TF-IDF), Similarity Metrics – Cosine similarity, Matrix Factorization methods – Singular Value Decomposition and Clustering are implemented showcase how different the different types of recommender systems answer various questions and the differences between the approaches. The methods are evaluated using Root Mean Squared Errors (RMSE scores) and hit rates against recommended movies.

![Movie Poster](/images/movies.jpg)

#### Goals
* Generate movie recommendations based on a particular Genre
* Generate movie recommendations based on Movie Similarity
* Generate movie recommendations based on User Similarity
* Generate movie recommendations based on a user’s Past Preferences 

#### Data
The MovieLens Latest Dataset is used which consists of 4 dataset files written in comma-separated values. Prior official permission to use the dataset for this project was obtained from GroupLens. The datasets, ‘movies.csv’ and ratings.csv’ are merged the final dataset explores 9742 unique movies, with over 100,000 ratings provided by 610 users. The dataset can be found on the [GroupLens Official Website](https://grouplens.org/datasets/movielens/).

#### Implementation
1.	Content-based Filtering – Using TF_IDF and Cosine Similarity Metric
2.	Collaborative Filtering
    - Memory-based – Using Cosine Similarity
      * Item-based
      * User-based
    - Model-based
      * Singular Value Decomposition
      * KNNBasic
      * KNNWithMeans

#### Tools and Technology
1. Python 3.8.5
   - **Libraries & Packages**: NumPy, Pandas, Matplotlib, Sklearn, Surprise
3. Jupyter Notebook (Anaconda) 

#### Key Findings

#### Conclusion
Recommender Systems offer personalization and help in increased profits for companies and also allow users to find the most relevant products for their use. The goal of the project to achieve a high-level understanding of the various filtering methods and their subsequent technologies was accomplished. The literature survey explored the various techniques and their advantages and disadvantages which further guides in selecting better models and evaluation metrics depending on the data. Implementing content-based filtering allowed to solve the cold-start problem that posed as a restriction for collaborative filtering. However, Faster and efficient results were achieved using model-based collaborative filtering, compared to both memory-based methods and content-based filtering. The project also posed certain challenges including finding proper evaluation methods/metrics for Top-N recommendations, however, hit rate was used similar to precision metric. A hybrid approach and implementation of deep learning techniques can further improve the accuracy and efficiency of recommender systems.

#### Future Work
This project covers the understanding and implementation of the basic techniques used to build a simple recommender system. Recent research suggests that using hybrid models, deep learning technologies such as RNNs and extensive hyperparameter tuning of existing models can increase the scalability, performance, and efficiency of these systems. New hybrid technologies may also solve existing issues with individual methods. Furthermore, evaluation of the Top-N recommendations gave lower hit rates implying the lack of implicit ratings and meta data on movies and users. Hence, larger amount of detailed data can help provide even more personalized recommendations. 
