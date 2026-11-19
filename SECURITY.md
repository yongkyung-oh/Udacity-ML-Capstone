# Installation and use

Use Python 3.11 in a separate virtual environment:

```sh
python3.11 -m venv .venv
. .venv/bin/activate
python -m pip install -r requirements.txt
python -m nltk.downloader punkt_tab
python naivebayes.py dev_text.txt dev_label.txt heldout_text.txt heldout_pred_nb.txt
```

Supply your development text, labels and held-out text files.

`requirements_nn.txt` adds PyTorch for importing the `RNN` class from `neuralnet.py`. Neural prediction requires compatible torchtext.data.Iterator. Training also requires torchtext.data/vocab APIs, pandas.DataFrame.append, matplotlib and weights-only PyTorch checkpoint loading; W2V requires gensim Word2Vec(size=...). The installation instructions apply to the Python scripts, not the notebooks.

Use trusted input files and tokenizer resources. Do not load untrusted serialized models or embeddings.
