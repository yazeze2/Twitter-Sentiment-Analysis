# Supervised Learning Sentiment Analysis on Tweets - The goal is to identify hate tweets. 

In this project I implemented various (listed below) supervised learning methods for sentiment analysis on tweets (a binary classification problem). The dataset can be acquired [here](https://datahack.analyticsvidhya.com/contest/practice-problem-twitter-sentiment-analysis/). Moreover, I have included the 'positive-words.txt' and 'negative-words.txt files in the data folder of this repository. These text files are used to devise and validate the Baseline Model (which is also provided here).

## Contents

### Pre-process data
    Process data to remove and replace characters and words irrlevant for analysis to create a processed training and testing data.
 
### Models
  - **Baseline Model** - This model basically draws the baseline for our model by making predictions solely based on the count of labelled positive words and negative words in a given tweet. If the number of positive words is greater than the negative, it can be concluded that the tweet is a positive tweet and vice versa. As a text file for both postive and negative words is provided along with the training and testing files, this baseline model relies entirley on the given sets. However, the results can be used to later judge the robustness of the machine learning models.



