# Natural Language Processing  - Sentiment Analysis on Tweets using Supervised Learning Algorithms (without using NLTK's in-built sentiment analysis engine)

In this project I implemented various (listed below) supervised learning methods for sentiment analysis on tweets (a binary classification problem). The dataset can be acquired [here](https://datahack.analyticsvidhya.com/contest/practice-problem-twitter-sentiment-analysis/). Moreover, I have included the 'positive-words.txt' and 'negative-words.txt files in the data folder of this repository. These text files are used to devise and validate the Baseline Model (which is also provided here).

## Contents

### Tools Required
The general requirements for this project are as follows:
- nltk
- regex
- numpy
- pandas
- matplotlib
- sci-kit learn
- scipy
- wordcloud

### Pre-process data
Process data to remove and replace characters and words irrlevant for analysis to create a processed training and testing data.
- **Process Word with regex**: Remove punctuations, Convert more than 2 letter repetitions to 2 letter, Check if word begins with an alphabet, and lowercase all the words
- **Process Emoticons using regex**: Replace emoticons with strings 'positive' or negative'
- **Process Tweet with regex:** Remove twitter usernames beginning with @, remove URLs, and replace #hashtag with hashtag

### Models & Validation Accuracies
  - **Baseline Model** - This model basically draws the baseline for our model by making predictions solely based on the count of labelled positive words and negative words in a given tweet. If the number of positive words is greater than the negative, it can be concluded that the tweet is a positive tweet and vice versa. As a text file for both postive and negative words is provided along with the training and testing files, this baseline model relies entirley on the given sets. However, the results can be used to later judge the robustness of the machine learning models. **Accuracy** = 20.03%
  - **Naive Bayes** - Accuracy = 94.28%
  - **SVM** - Accuracy = 95.21%
  - **Naive Bayes** - Accuracy = 97.8%
