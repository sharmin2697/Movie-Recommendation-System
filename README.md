## MOVIE RECOMMENDATION SYSTEM - USING MOVIELENS DATA

#### About
Personalized recommendations are of key importance when it comes to increasing business value and sales of products, along with customer retention and satisfaction. Companies generate higher revenues and save resources, by simply understanding individual customer behaviors. In recent times, a large portion of the information we see online, comes from recommendations catered to us based on content or products we have previously liked or invested in. Grouping similar users or items can allow for vast exposure of products to multiple users. Recommender systems are mainly of 2 types – Content-based Filtering and Collaborative Filtering (Memory-based and Model-based). Using both Implicit and Explicit ratings, companies can recommend relevant content to its users. 

This project aims to build a movie recommendation system that utilizes explicit ratings and movie genres to make personalized recommendations. Machine Learning methods including Term Frequency and Inverse Document Frequency (TF-IDF), Similarity Metrics – Cosine similarity, Matrix Factorization methods – Singular Value Decomposition and Clustering is implemented, to showcase how different the different types of recommender systems answer various questions and the differences between the approaches. The methods are evaluated using Root Mean Squared Errors (RMSE scores) and hit rates against recommended movies.

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

#### Contents
1. **code** - This folder contains the main code to build the recommender system
   * Functions.ipynb: *All function used in the following notebooks*
   * Data Pre-Processing.ipynb: *Data cleaning and pre-processing*
   * EDA.ipynb: *Code for visualizations*
   * Content Based Filtering.ipynb: *Code to build recommender system using tf-idf and cosine similarity*
   * Collaborative Filtering Memory Based.ipynb: *Code to build recommender system using item-based and user-based approach* 
   * Collaborative Filtering Model Based.ipynb: *Code to build recommender system using matrix factorization and clustering methods*
2. **data** - This folder contains the datasets of MovieLens 
3. **images** - This folder contains images used to build GitHub Pages
4. **report & presentation** - This folder contains the final report and presentation for this capstone project

#### Notes
- Install the following libraries before running the notebooks:
  > pip install scikit-surprise
  
  > pip install import-ipynb


### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sharmin2697/Movie-Recommendation-System/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
