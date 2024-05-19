# Movie Recommender System

This Jupyter notebook, `movie_recommender.ipynb`, provides an extensive exploration and implementation of several movie recommendation algorithms. The notebook covers user-based and item-based collaborative filtering, matrix factorization techniques like SVD, and a basic movie average based system.

## Dataset Overview

The dataset consists of 6040 users and 3706 unique movies, formatted in `.dat` files. The data is imported into the Jupyter Notebook using the Pandas library with ISO-8859-1 encoding to maintain the readability of text data.

## Features

### Recommendation Techniques

1. **K-Nearest Neighbors Collaborative Filtering (KNNCF)**
   - User-based collaborative filtering with tunable K values.
   - Evaluation metrics include RMSE, Average Precision (AP), and Normalized Discounted Cumulative Gain (nDCG).

2. **Item-based Collaborative Filtering**
   - Techniques: Pearson Correlation and Cosine Similarity.
   - Effectiveness assessed using RMSE for different similarity measures.

3. **Matrix Factorization**
   - Utilizes Single Value Decomposition (SVD) from the Surprise library.
   - Capable of handling sparse data and providing personalized recommendations.

4. **Movie Average System**
   - Simple approach based on the mean rating of movies.
   - Recommended for users with a history of more than 100 movie ratings.

### Evaluation Metrics

- **Average Precision (AP)**
- **Normalized Discounted Cumulative Gain (nDCG)**
- **Root Mean Square Error (RMSE)**

## Installation

Ensure you have Python 3.x installed along with Jupyter Notebook or JupyterLab. Required libraries can be installed via:

```bash
pip install pandas matplotlib scikit-surprise
