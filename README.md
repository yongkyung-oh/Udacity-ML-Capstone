# Udacity-ML-Capstone

## Project Overview
Sentiment classification, detecting if a piece of text is positive or negative, is a common NLP task that is useful for understanding feedback in product reviews, user's opinions, etc. Sentiment can be expressed in natural language in both trivial and non-trivial ways.
In this project, I build two sentiment classifiers based on Naive Bayes and neural networks. Because of the lack of train data, I conducted pre-process and random sampling. After that, I develop two classifiers. For Naive Bayes, I use the TF-IDF as feature of train data. The main model is based on MultinomialNB. In case of neural net, I compared word embedding from train data and pretrained embedding(Glove 6B). The main model is based on bi-directional LSTM. Both classifiers work well and acheive the target accuracy.

## Code

```sh
python naivebayes.py dev_text.txt dev_label.txt heldout_text.txt heldout_pred_nb.txt
```

Use Python 3.11 with `requirements.txt` for Naive Bayes. `requirements_nn.txt` adds PyTorch for RNN module use. Neural prediction requires compatible torchtext.data.Iterator. Training also requires torchtext.data/vocab APIs, pandas.DataFrame.append, matplotlib and weights-only PyTorch checkpoint loading; W2V requires gensim Word2Vec(size=...). See [Installation and use](SECURITY.md).

## Project Result
[NB Model](https://github.com/yongkyung-oh/Udacity-ML-Capstone/blob/master/naivebayes.ipynb)

[NN Model-W2V](https://github.com/yongkyung-oh/Udacity-ML-Capstone/blob/master/neuralnet-W2V.ipynb)

[NN Model-G6B](https://github.com/yongkyung-oh/Udacity-ML-Capstone/blob/master/neuralnet-G6B.ipynb)
