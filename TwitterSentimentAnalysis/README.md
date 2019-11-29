
#Twitter Sentiment Analysis

This is competition hosted by Analytics Vidhya to analyze the sentiments of the twitter comments.

Problem Statement : 

The objective of this competition is to detect hate speech in tweets. For the sake of simplicity, we say a tweet contains hate speech if it has a racist or sexist sentiment associated with it. So, the task is to classify racist or sexist tweets from other tweets.

Approach: 

To classify the racist or sexist tweets from other tweets we can use machine learning classification algorithms like Logistic Regression, Random Forest, Naive Bayes, Support Vector Machine etc. Before the model development we need to understand and extract features from data as its unstructured data. We need to use text classification methods to process the data. 
The following are the steps involved in the Project - 

1. Understanding the data : 

Before processing the data, we need to understand the data. We see that training data consists of three columns - Id, label and tweets. Label tells us whether the tweet is racist or not. We notice that 74.5 percent of comments are non - racist. 

2. Data Preprocessing :

 In any natural language processing task, cleaning raw text data is an important    step. It helps in getting rid of the unwanted words and characters which helps in obtaining better features. If we skip this step then there is a higher chance that you are working with noisy and inconsistent data. The objective of this step is to clean the noise those are less relevant to find the sentiment of tweets such as punctuation, special characters, numbers, and terms which don’t carry much weightage in context to the text. These are following processing that I have done-

 a. Removing the words starting with @ - These words are the names of the used which will not help us in classification. So we can remove all the words starting with @
 
 b. Removing the punctuation, numbers and special characters.
 
 c. Removing the urls in the tweets- We notice that there are many urls and links in the text, so we can remove that as they do not seem important for the model
 
 d. Removing the short words whose length is less than 3. 
 
 e. Removing the stop words - Stop words consists of common words link the, of, about etc. which can be removed.
 
 f. Text Normalization - Text normalization is the process of finding the root words like making becomes make. This groups the words    that have the same meaning but are in different forms. This can be done with the help of nltk package. 

3.Visualizing the Tweets 
 
This step is to understand which words appear most frequently in the tweets. It also helps us to understand which words might mostly contribute to the type of tweet. As we know there are many hashtags present in the tweets. These hashtags sometimes help us to understand the sentiment of the user. So we can look at hashtags that are most frequent in racist comments vs non racist comments. 
Extracting features from the tweets
 
There are many different methods to extract features from tweets. They are -    Bag of Words, TF-IDF, and Word Embeddings. We will use all the methods and then check which methods gives us better performance.

a. Bag of Words

b. TF- IDF

c. Word Embeddings 


4. Model Development and Evaluation
 


