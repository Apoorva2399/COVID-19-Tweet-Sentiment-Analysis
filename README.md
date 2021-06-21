# COVID-19 Tweet Sentiment Analysis

### Problem Description : 

This challenge asks you to build a classification model to predict the sentiment of COVID-19 tweets.The tweets have been pulled from Twitter and manual tagging has been done then. The names and usernames have been given codes to avoid any privacy concerns.

### Data Description :

You are given the following information:
Location
Tweet At
Original Tweet
Label

### Data Preprocessing : 
* The preprocessing of the text data is an essential step as it makes the raw text ready for mining.
* The objective of this step is to clean noise those are less relevant to find the sentiment of tweets such as punctuation, special characters, numbers, and terms which don’t    carry much weightage in context to the text.
* The tweets contain lots of twitter handles (@user). We will remove all these twitter handles from the data as they don’t convey much information.
* We have analyzed that most of the tweets are like #coronavirus #covid-19 and this tweets are almost present in all the sentiments. So there is no use of keeping these      hashtags in text. It will make the data noisy and which will affect accuracy of model.
* We are having twitter links in the data which are not useful for our Model. It will make our data noisy.
* Punctuations, numbers and special characters do not help much. It is better to remove them from the text just as we removed the twitter handles,links and hashtags.
* Stop words are those words in natural language that have a very little meaning, such as "is", "an", "the", etc.To remove stop words from a sentence, you can divide your text into words and then remove the word if it exits in the list of stop words provided by NLTK.
* Stemming is a rule-based process of stripping the suffixes (“ing”, “ly”, “es”, “ed”, “s” etc) from a word. For example – “play”, “player”, “played”, “plays” and “playing” are the different variations of the word – “play”.
* Lemmatization is a more powerful operation, and it takes into consideration morphological analysis of the words. It returns the lemma which is the base form of all its inflectional forms.
* In tokenization we convert group of sentence into token . It is also called text segmentation or lexical analysis. It is basically splitting data into small chunk of words. Tokenization in python can be done by python NLTK library’s word_tokenize() function.
* We chose Count Vectorizer as our Vectorizer with minimum  document frequency =10. It will create a sparse matrix of all words and the number of times they are present in a document.

### Conclusion
* For multiclass classification, the best model for this dataset would be CatBoost
* For binary classification, the best model for this dataset would be Stochastic Gradient Descent





