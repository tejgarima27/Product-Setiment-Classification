# Product-Setiment-Classification (or) Sentiment-Classification-for-Product-Reviews

Analysing sentiments related to various products such as Tablet, Mobile and various other gizmos can be fun and difficult especially when collected across various demographics around the world. The aim is to develop a machine learning model to accurately classify various products into 4 different classes of sentiments based on the raw text review provided by the user. Analysing these sentiments will not only help to serve the customers better but can also reveal lot of customer traits present/hidden in the reviews.

The sentiment analysis requires a lot to be taken into account mainly due to the pre-processing involved to represent raw text and make them machine-understandable. Usually, we perform stemming and lemmatization to the raw information and then represent it using TF-IDF, Word Embedding’s, etc. However, provided the state-of-the-art NLP models such as Transformer based BERT models one can skip the manual feature engineering like TF-IDF and Count Vectorizers.So,the task of this dataset is to correctly classify product description sentiments.

### OBJECTIVE: TO INVESTIGATE BEST SUITED SUPERVISED TECHNIQUE FOR CLASSIFICATION OF PRODUCT DESCRIPTION SENTIMENTS.

#### Attribute Description:
* TextID - Unique Identifier Product 
* Description - Description of the product review by a user
* Product_Type - Different types of product (9 unique products)
* Class - Represents various sentiments(4 NOMINAL CLASSES)

* 0 - Cannot Say
* 1 - Negative
* 2 - Positive
* 3 - No Sentiment


* Sentiment analysis also called as opinion mining is a subfield within Natural Language Processing (NLP) that builds machine learning algorithms to classify a text according to the sentimental polarities of opinions it contains, e.g., positive or negative. In recent year, sentiment analysis has become a topic of great interest and development in both academics and industry. Analysing the sentiment of texts could benefit, for example, customer services, product analytics, market research etc. Take Amazon as an example. Customers on Amazon platform choose their preferred products based on the reviews from other users. an automatic sentiment classification system can not only help companies grasp the satisfaction level of the products, but also significantly assist new customers to locate their online shopping shelves.The problem of learning the sentimental polarities of opinions is reduced to the Classification problem. There are many machine learning methods that can be used in the classification task. They can be categorised into supervised method (like SVM) and unsupervised method (like clustering). In this snippet their is usage of only Supervised Machine learning Algorithm.
The Supervised Learning Algorithm which is used over this task is Multi-Nomial Logistic Regression on Unigram, Bigram and then TF-IDF vector to compare thier performances on same task.Multinomial logistic regression is used when the dependent variable in question is nominal (equivalently categorical, meaning that it falls into any one of a set of categories that cannot be ordered in any meaningful way) and for which there are more than two categories.

* The aim of this challenge is to develop a sentiment classifier that can assign a large set of product reviews to the four levels of polarity of opinion as accurately as possible. It is a multi-class classification task, where each product review is labeled with one of the four sentiment labels, which are indicated by 0,1,2 & 3 described above.

### CONCLUSION
Metrics:
* 1.MULTINOMIAL LOGISTIC REGRESSION ON UNIGRAM MODEL - Accuracy:0.64257
* 2.MULTINOMIAL LOGISTIC REGRESSION ON BIGRAM MODEL - Accuracy:0.66928
* 3.MULTINOMIAL LOGISTIC REGRESSION ON TF-IDF VECTOR MODEL - Accuracy:0.60015
We have successufully modeled the text classifier to predict the sentiment of a product review.

* The MULTINOMIAL LOGISTIC REGRESSION ON BIGRAM MODEL gave the highest accuracy among 3 of aroud 70%.
As for further improvement we could apply different Transfer Learning models to train this model to get better results in short span of time.
