
## Minimum Viable Product (MVP) - Tweets Sentiment Analysis

The goal of this project is to perform sentiment analysis for Covid19 related tweets.

### Solution Path
To do this, I'm using more than 40k tweets collectd between March 2020 and April 2020. Supervised classification will be performed based on the existed sentiment categories using the classification tools from the last module. Unsupervised topic modeling will be performed as well as Dynamic topic modeling.

### Work Completed
In pre-processing the data, I removed all digits and punctuation, I used nltk.corpus to remove stop words. Also, the tweets contains a lot of accent words and fractions, which were removed as well.

After data preprocessing, I created a baseline classification model using CountVectorizer and Logistic Regression. 

I also created a baseline topic modeling model using CountVectorizer and NMF topic modeler with a small number of topic components (n=10).

### Recent Findings
 - Classification model
   I got the confusion matrix below with 5 targets:
   ![](image.png) 
 - NMF topic modeler
   I got the 10 topic components with the most related 10 words for each components as well as the wordcloud plot:
   
['chain-going-local-bank-buy-supply-demand-stock-panic-food',
 'day-went-work-thank-today-retail-going-like-grocery-store',
 'positive-market-response-help-crisis-impact-outbreak-spread-retail-covid',
 'delivery-work-time-today-day-going-like-local-staff-supermarket',
 'really-time-dont-buy-stop-think-going-like-panic-people',
 'health-spending-impact-time-crisis-protection-business-behavior-new-consumer',
 'support-local-going-grocery-shop-like-new-time-delivery-shopping',
 'went-water-panic-buy-roll-stock-like-hand-toilet-paper',
 'buy-make-safe-time-work-hand-help-stay-home-need',
 'market-low-supply-new-price-global-amid-oil-demand-pandemic']
 
   ![](image.png) 
   - Prelim findings for Dynamic topic modeling
     I plot the time series for the number of tweets everyday of the 5 sentiment categories, there are interesting trends that can lead to Dynamic topic modeling in the next stage.
     ![](image.png) 
### Moving Forward
I will continue with better topic modeling tools that can anchor the certain selected topics. I will continue with dynamic modeling to find out the trends of tweet sentiment related to Covid daily cases.
