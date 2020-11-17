# Sentiment Analysis using NLP
Sentiment Analysis on iMDB movie reviews and classifying them into 2 labels : Positive and Negative using various ML models.

iMDB Movie Review Dataset : https://ai.stanford.edu/~amaas/data/sentiment/

## Steps
1 - DataFrame Creation : First of all, we created a pandas dataframe consisting of 2 columns, text and label, from the raw data files.  
2 - Preprocessing : We carried out preprocessing on the data . The steps include - removal of blank rows, changing all text to lower case, tokenization, stop words removal, numeric and special characters removal, POS tagging, word stemming/lemmatization.  
3 - Train Test Split : We divided our dataset into training and testing data in 80-20 ratio  
4 - Pipelines : We defined various pipelines,i.e, sequentially applied a list of transforms and a final estimator. The basic structure of the pipelines are CountVectorizer->TFIDFVectorizer->Model(). The models we used are listed below.   

Overview of different accuracies:
![accuracy list](https://user-images.githubusercontent.com/53677987/99288966-5a310480-2862-11eb-96df-e59f7bc60c28.jpg)

