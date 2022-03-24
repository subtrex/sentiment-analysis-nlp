# Sentiment Analysis using Natural Language Processing (NLP)

Sentiment Analysis on IMDb Movie Reviews dataset using Natural Language Processing, classifying them into 2 labels: Positive and Negative.

## Tech

Python | NLTK | TensorFlow | Keras

## Data

We made use of the [IMDb Movie Reviews dataset](https://ai.stanford.edu/~amaas/data/sentiment/).

## Methodology

1 - DataFrame Creation : We created a pandas dataframe consisting of 2 columns, text and label, from the raw data files.  
2 - Preprocessing : We performed certain preprocessing steps on the text corpus, which included removal of blank rows -> changing all text to lower case -> tokenization -> stop words removal -> numeric and special characters removal -> POS tagging -> word stemming/lemmatization.  
3 - Train Test Split : We divided our dataset into training and testing data in 80:20 ratio.  
4 - Pipelines : We defined various pipelines i.e. sequentially applied a list of transforms and a final estimator. The basic structure of the pipelines are CountVectorizer -> TFIDFVectorizer -> ClassifierModel. Then we trained the pipeline on the training data and used the testing data for prediction results.   

## Results

| Classifier  | Accuracy(%) |
| ------------- | ------------- |
| Logistic Regression  | 89 |
| Stochastic Gradient Descent  | 85  |
| Multinomial Naive Bayes | 86 |
| SVM (Linear) | 89 |
| Decision Tree | 71 |
| Extra Tree | 64 |
| Multilayer Perceptron | 89 |
| Ridge Classifier | 88 |
| AdaBoost| 82 |
| GradBoost | 80 |
| Random Forest | 75 |
