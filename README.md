# **Natural-Language-Processing-with-Disaster-Tweets**
Predicting tweets about real disaster with the help of machine learning and NLP

## **Dataset description**
Original dataset can be found here: https://www.kaggle.com/competitions/nlp-getting-started/data \
Whole dataset is divided into modeling data (labeled) and oot data (unlabeled)

Modeling data is further divided into train-test in a 75:25 ratio which contains:
> A **text** of tweet\
> A **keyword** from the tweet\
> A **location** from where the tweet was sent\
> A **label: 1/0** (1 if it is disaster tweet else 0)

## **Approach**

Text processing is done by TFIDF vectorization with a vector of size 2000\
Ordinal encoded keyword and location so we can use them as features in modeling

CatBoost Classifier is used for modeling since it is good with handling categorical variables

## **Performance**

Performance on test data for predicting disaster tweet:

> Precision: 0.87\
> Recall: 0.62\
> F1: 0.72
