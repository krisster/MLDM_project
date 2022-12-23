# MLDM_project

We, Kristina Denisova and Tatyana Shelovanova, try to create a recommendation system according to purchases from H&M data

Welcome!

The main page for the competition https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/overview

### Dataset Description
For this challenge you are given the purchase history of customers across time, along with supporting metadata. Your challenge is to predict what articles each customer will purchase in the 7-day period immediately after the training data ends. Customer who did not make any purchase during that time are excluded from the scoring.

### Files

- **images** - a folder of images corresponding to each article_id; images are placed in subfolders starting with the first three digits of the article_id; note, not all- article_id values have a corresponding image (we decide not to use them)
- **articles.csv** - detailed metadata for each article_id available for purchase
- **customers.csv** - metadata for each customer_id in dataset
- **sample_submission.csv** - a sample submission file in the correct format
- **transactions_train.csv** - the training data, consisting of the purchases each customer for each date, as well as additional information. Duplicate rows correspond to multiple purchases of the same item. 

**Your task is to predict the article_ids each customer will purchase during the 7-day period immediately after the training data period**

### Project progress

- **Nov, 19** - the intermidiate report where we make statistics according to data and evaluate KMeans
- **Dec, 1** - the data cut and evaluation of model according top-popular item list
- **Dec, 3** - added methods of collaborative filtring
- **Dec, 23** - add more deepen methods of collaborative filtering: use KNN and ALS. Unfortunetaly, ALS doesn't work properly

**Modifications**

Additionally to our previous report we add a simple model of recommendations according to popularity among users. So, get the same recommended items for all users

Also we have tried to provide a collaborative filtering model to predict recommendations according to similarity of items among users. To do this we use a cosine similarity 

For final model we'd like to a little bit modify KMeans method and individualize predictions using a previous collaborative filtering method (now we have the same recommendations for all)

**Updated**
For the last version we have models (collaborative filtering with KNN and ALS) that make individual predictions based on the similarity of items. So, for example, if I bought black jeans I will be interested in bluejeans but different model

However, we have two problems: the first one is that this scheme maybe relevant for books/films. But it is better to find similar customers and recommend to buy things that they haven't bought. The second one is that ALS doesn't work correctly
