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
