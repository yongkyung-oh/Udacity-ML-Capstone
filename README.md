# Udacity-ML-Capstone

## Project Overview
Sentiment classification, detecting if a piece of text is positive or negative, is a common NLP task that is useful for understanding feedback in product reviews, user's opinions, etc. Sentiment can be expressed in natural language in both trivial and non-trivial ways.
In this project, I build two sentiment classifiers based on Naive Bayes and neural networks. Because of the lack of train data, I conducted pre-process and random sampling. After that, I develop two classifiers. For Naive Bayes, I use the TF-IDF as feature of train data. The main model is based on MultinomialNB. In case of neural net, I compared word embedding from train data and pretrained embedding(Glove 6B). The main model is based on bi-directional LSTM. Both classifiers work well and acheive the target accuracy.

## Code

`naivebayes.py dev_text.txt dev_label.txt heldout_text.txt heldout_pred_nb.txt`

`neuralnet.py dev_text.txt dev_label.txt heldout_text.txt heldout_pred_nn.txt`

requirments.txt - for naivebayes.py
requirments_nn.txt - for neuralnet.py

- Tested on ubuntu 16.04
- Used 'python' rather than 'python3'
- In the neuralnet.py, I used cuda:1 instead of cuda:0 due to hardware issue

## Project Result
[NB Model]()

[NN Model-W2V]()

[NN Model-G6B]()
