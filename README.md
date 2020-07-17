# Toxic-Comment-Classification
![Competition](https://github.com/nischaygowda105/Toxic-Comment-Classification-Challenge-Jigsaw/blob/master/competition.png)
## Toxic Comment Classification Challenge, Kaggle Competion by Jigsaw 

[Kaggle Competition link](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/overview)

In this competition, you’re challenged to build a multi-headed model that’s capable of detecting different types of of toxicity like threats, obscenity, insults, and identity-based hate

## Dataset 
You’ll be using a dataset of comments from Wikipedia’s talk page edits. You are provided with a large number of Wikipedia comments which have been labeled by human raters for toxic behavior. The types of toxicity are:

    -toxic
    -severe_toxic
    -obscene
    -threat
    -insult
    -identity_hate
    
You must create a model which predicts a probability of each type of toxicity for each comment.
[Data link](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data)

## Steps followed.

Steps I followed to approach the problem and get the desired output.

### 1. Explore Data
  Simple data exploration operations like count, unique class, and also null values check.
  
  1. Empty Comments replacemnet with 'Unknown'.
  
  2. Empty labels - replaced with 'None'.
  
### 2. Model Build.
  Steps involve converison of sentences to word tokens and draw insights to train model and predict the label probaility.
  
  1. Regex -  to remove all unwanted punctuations and special characters.
  
  2. Tokenize - split sentences to words.
  
  3. TfIdf Vectorizer - assigns feature values to words based on theier occurance.
  
  4. Logitstic Regression - to calculate the probability of each class, for every given test datapoint.


