# Sarcasm-Detection

A repository for the final project of Neural Natural Language Processing course at Skoltech.

In this project we wanted to identify sarcasm in online comments. It is an interesting and non-trivial NLP task, with which we wanted to get acquainted in our project. In addition to building the classification model, we also wanted to analyze what distinguishes sacrasm from normal text.

The main questions of our project: **Can sarcasm can be identified with a good accuracy? What differs sarcasm from usual language?**

Dataset: https://www.kaggle.com/danofer/sarcasm

This is the main dataset that we used. It contains ~1.3M comments from Reddit, and an important thing is that the data is balanced.

The metric used to measure model quality on validation data was AUC-ROC in order to work with probabilities of classes, not with just predictions of classes.

Final notebook with all the results: https://github.com/blacKitten13/Sarcasm-Detection/blob/master/final_notebook.ipynb

Model results:

|Model|AUC-ROC|
|-|-|
|BiLSTM + GloVe|0.809782|
|BiLSTM + ELMo|0.808948|
|LR + TF-IDF|0.794278|
|BiLSTM + Word2Vec|0.794272|
|LR + CntVectorizer|0.787733|
|LR + Doc2Vec|0.677191|
|LR + GloVe|0.674855|
|LR + Word2Vec|0.673213|
