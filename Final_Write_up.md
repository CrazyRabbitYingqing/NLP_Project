## NLP Project - COVID-19 Tweets Topic Modeling & Sentiment Analysis

Yingqing Qiu, Feburary, 2022

### Abstract

This NLP unsupervised learning project will answer the question about the hot topics and the sentiment of the twitter users to Covid-19 at the beginning of the pandemic. With the topic modeling and sentiment analysis results, social scientists and psychologists can proceed with studies on how people express emotions and sentiments and what they most care about when dealing with catastrophic events for the usage of future government policymaking. This project adopts topic modeling, dynamic topic modeling, and sentiment analysis python packages. The conclustions include the selection of the most efficient topic modeling technique, interpretive of the Five (5) most related topics and the time evolution of these topic probabilities, as well as the sentiment predictions. Further evaluations and discusstions will be provided during the presentation.

### design

First, the data set was preprocessed with python packages, including removing punctuation marks, website URLs, numerics, and accent alphabet. After the preprocessing, the tweets were vectorized then became sparse matrices for further topic modeling. Multiple topiv modeling techniques were examined to generated the top five most reasonable topics. Meanwhile, dynamic topic modeling technique was also applied to study the possibilities of the topics during the time span.In the end, a sentiment analysis was performed to support the analysis.

### data
### algorithms
### tools
### communication


Data Description:
I plan to use a dataset from Kaggle

The data set title: Coronavirus tweets NLP

The dataset including columns: Tweet Location, Time, Twitter Text, Sentiment Label

The entire dataset contains more than 40k unique Twitter texts that posted between mid-March to mid-April 2020

Supplemental data: Covid daily cases at the Tweet locations

I will use the dataset to build an unsupervised learning model including dimensionality reduction/topic modeling and clustering in Python.

Also, supervised modeling methods like some classification models will be practiced as a comparison.

Tools:
Python text processing libraries/ tools: NLTK, spaCy, gensim, sklearn

Visualization: seaborn

