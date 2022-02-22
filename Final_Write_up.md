## NLP Project Final Write-up - COVID-19 Tweets Topic Modeling & Sentiment Analysis

Yingqing Qiu, Feburary, 2022

### Abstract

This NLP unsupervised learning project will answer the question about the hot topics and the sentiment of the twitter users to Covid-19 at the beginning of the pandemic. With the topic modeling and sentiment analysis results, social scientists and psychologists can proceed with studies on how people express emotions and sentiments and what they are most caring about when dealing with catastrophic events for the usage of future government policymaking. This project adopts topic modeling, dynamic topic modeling, and sentiment analysis python packages. The conclustions include the selection of the most efficient topic modeling technique, interpretive of the Five (5) most related topics and the time evolution of these topic probabilities, as well as the sentiment predictions. Further evaluations and discusstions will be provided during the presentation.

### Design

First, the data set was preprocessed with python packages, including removing punctuation marks, website URLs, numerics, and accent alphabet. After the preprocessing, the tweets were vectorized then became sparse matrices for further topic modeling. Multiple topic modeling techniques were examined to generate the top five most reasonable topics. Meanwhile, dynamic topic modeling technique was also applied to study the possibilities of the topics during the time span. In the end, a sentiment analysis was performed to support the analysis.

### Data

Data set: Kaggle data set - [Coronavirus tweets NLP](https://www.kaggle.com/datatattle/covid-19-nlp-text-classification)

The dataset including columns: Tweet Location, Time, Twitter Text, Sentiment Label

The entire dataset contains more than 40k unique Tweet documents that posted between early-March to mid-April 2020 when the COVID Cases start to rise up in the United States.

Supplemental data: Covid daily cases from [NYTimes_github](https://github.com/nytimes/covid-19-data/blob/master/us.csv).

### Algorithms

First, Data set preprocessing was conducted using NLTK LancasterStemmer, NLTK stopwords package, python remove function, and pandas dropna function. Second, text vectorization was conducted with both CountVectorizer and TF-IDF Vectorizer, the ngram was set to only one word. Third, two topic modeling tools were adopted: NMF and LSA, in which the tools applied with TF-IDF Vectorizer data ran slow. Fourth, Dynamic topic modeling was performed by python gensim ldaseqmodel for the text set during 44 days, the model runs for 7 hours. In the end, VADER SentimentIntensityAnalyzer was adopted to predict the sentiment of the tweets.

Final Topic Modeling tool selected: TF-IDF Vectorizer + NMF

Five selected Topics:

Topic 1 - "Panic"

'demand, need, panic, stock, food, hoard, bank'

Topic 2 - "Grocery"

'like, go, work, groceri, store, local, today, day, shop'

Topic 3 - "Retail"

'impact, pandem, shop, consum, covid, protect, retail, oil, outbreak'

Topic 4 - "Social" 

'time, work, shop, peopl, supermarket, social, home, staff'

Topic 5 - "Toilet Paper"

'roll, peopl, hand, toilet, paper, buy, shortag, water, hoard'

### Tools
Python libraries:

NLTK, re, gensim, sklearn, numpy, vaderSentiment

Visualization: 

Matplotlib, Canvas built-in pie plotter

### Communication

The presentation slides contain all the results visulization and interpretation.


