# Emotion-Detection-From-Tweets-Using-BERT-and-SVM

This code accompanies the paper "**Emotion detection from tweets using a BERT and SVM ensemble model**" published in U.P.B. Sci. Bull., Series C, Vol. 84, Iss. 1, pp. 63-74, 2022.

[Paper link here.](https://www.scientificbulletin.upb.ro/rev_docs_arhiva/rez982_619644.pdf)

## Description

A novel BERT-SVM ensemble model for the task of emotion detection is introduced. This model achieves state-of-the-art performance on the dataset offered at [WASSA-2017 Shared Task on Emotion Intensity](https://www.academia.edu/67783420/WASSA_2017_Shared_Task_on_Emotion_Intensity).  
On top of this, we enhance the current dataset by adding a new class, the **neutral** class, which has been shown to be a good practice when working with real life data.


## Model training

### Training the SVM model

The **SVM** model is the first that must be trained. After saving the model using the pickle library, the model has to be imported when creating the ensemble model.
The code for training the SVM model on WASSA dataset is inside the **SVM_wassa.ipynb** file.  
The **SVM.ipynb** contains the code for training the model capable of detecting **neutral** tweets. 

### Training the BERT model and the ensemble model
Three versions of **BERT** have been tested: vanilla BERT, RoBERTa and **BERTweet**.
For building the ensemble model is recommended training and using **BERTweet** as this flavour of BERT has been shown to offer best performance when working with tweets.  
The code for training the model on WASSA dataset is inside the **Bert_wassa.ipynb** file. Also the coresponding ensemble model for WASSA dataset is built here.  
The BERT and ensemble model able to detect neutral emotions can be trained using **Bert.ipynb**.
