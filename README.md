# Natural Language Processing:
### Sentiment Analysis on Tweets using Supervised Learning Algorithms (without using NLTK's in-built sentiment analysis engine)

**Algorithms:** Naive Bayes, Decision Tree, SVM

In this project I implemented various (listed below) supervised learning methods for sentiment analysis on tweets (a binary classification problem). The dataset can be acquired [here](https://datahack.analyticsvidhya.com/contest/practice-problem-twitter-sentiment-analysis/). Moreover, I have included the 'positive-words.txt' and 'negative-words.txt files in the data folder of this repository. These text files are used to devise and validate the Baseline Model (which is also provided here).

## Contents

### Tools Required
The general requirements for this project are as follows:
- nltk
- regex
- numpy
- pandas
- matplotlib
- scikit-learn
- scipy
- wordcloud
### Preprocessing
Process data to remove and replace characters and words irrlevant for analysis to create a processed training and testing .csv file.
- **Process characters/words of each tweet with regex**: Remove punctuations, Convert more than 2 letter repetitions to 2 letter, Check if word begins with an alphabet, and lowercase all the words
- **Process Emoticons using regex**: Replace emoticons with strings 'positive' or negative'
- **Process Tweet with regex:** Remove twitter usernames beginning with @, remove URLs, and replace #hashtag with hashtag

### Model Building & Validation Accuracy

- **Feature Extraction** - namely, unigrams and bigrams
- **Feature Representation** - Sparse Vector Representation for word 'presence' and 'frequency' feature types. the best results were obtained using the 'presence' feature except for the SVM model.
- **Classifiers**
    - **Baseline Model** - This model basically draws the baseline for our model by making predictions solely based on the count of labelled positive words and negative words in a given tweet. If the number of positive words is greater than the negative, it can be concluded that the tweet is a positive tweet and vice versa. As a text file for both postive and negative words is provided along with the training and testing files, this baseline model relies entirley on the given sets. However, the results can be used to later judge the robustness of the machine learning models. **Accuracy** = 20.03%
    - **Naive Bayes** - Accuracy = 79.68%
    - **Decision Trees** - Accuracy = 68.01%
    - **SVM** - Accuracy = 81.55% 
