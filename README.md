# Identify-the-Sentiments
#### Overview:
       Sentiment analysis is contextual mining of text which identifies and extracts subjective information 
       in source material, and helping a business to understand the social sentiment of their brand, product
       or service while monitoring online conversations.This was a practise problem given by Analytics Vidya.
       In this challenge, We are provided with tweet data to predict sentiment on electronic products of netizens.
       The metric used for evaluating the performance of classification model would be weighted F1-Score.
       
#### Dataset:
       The dataset was given by Analytics Vidya which is in .csv format.The dataset have three columns and 
       7920 observation.Out of three columns one represent the tweet ,one represent id and remaining one 
       represent the sentiment which is either 1(negative) or 0(positive).Out of 7920 observation 75% tweets 
       are positive sentiment while remaining are negative.
         
#### Preprocessing:
     The most important part of Sentiment analysis is preprocees the raw text data and extract informative 
     features from them for machine learning and deep learning model.Since the twet data are too messy ,so 
     I applied some of common preprocessing steps like
          1.Convert tweet into lower case letters
          2.Remove URL
          3. Remove HTML tags
          4.Convert all emoji and emoticons into text format
          5.Replace contractions  with respective full form
          6.Since there may be chart words in the data .So we need to replace them with meaningfull word
          7.Clean tweet data
          8. Remove Punctuations which are not ncessary for further analysis
          9.Spelling Correction
          10. Remove stopwords
          11.Stemming the tweet data 
# Model:          
        In this project I extracted features by using TfidfVectorizer , CountVectorizer and Word embedding 
        (glove & fasttext embedding vector).I applied various machine learning algorithimon both 
        countvectorizer and TfidfVectorizer with best model is Logistic Regression having accuracy 93% which 
        code can be found in the identify the sentiments.ipynb file. I applied RNN on glove embedding vector 
        as well as Fasttext.               
