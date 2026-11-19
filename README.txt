Use Python 3.11 and requirements.txt in a separate virtual environment.

python -m nltk.downloader punkt_tab
python naivebayes.py dev_text.txt dev_label.txt heldout_text.txt heldout_pred_nb.txt

requirements_nn.txt adds PyTorch for importing the RNN class.
Neural prediction requires compatible torchtext.data.Iterator. Training also requires torchtext.data/vocab APIs, pandas.DataFrame.append, matplotlib and weights-only PyTorch checkpoint loading; W2V requires gensim Word2Vec(size=...).
See the repository SECURITY.md for installation and use.
