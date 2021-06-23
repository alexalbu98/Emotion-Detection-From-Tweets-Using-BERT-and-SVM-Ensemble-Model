# Emotion-Detection-From-Tweets-Using-BERT-and-SVM

This code accompanies the paper "Emotion Detection from Tweets Using a BERT and SVM Ensemble Model".

## Description

A BERT and SVM approach for the task of emotion detection from tweets. A novel BERT-SVM ensemble model for the task of emotion detection is introduced.


## Model training

### Training the SVM model

The SVM model is the first that must be trained. After saving the model using the pickle library, the model has to be imported when creating the ensemble model.
All the code for the SVM model and Ensemble model is found in the SVM.ipynb file.

### Training the BERT model and the ensemble model
Three versions of BERT have been tried: vanilla BERT, RoBERTa and BERTweet.

For building the ensemble model is recommended training and using BERTweet when building the ensemble model.

All the code is found in Bert.ipynb file.
