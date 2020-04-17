# Experiments

In this directory, you will find two notebooks with my experiments for using BERT for Word Sense Induction. One should look at them in chronological order:

## 1. ConvBERT
In this notebook, I used DeepPavlov's conversational RuBERT model to obtain contextual embeddings for the target words, and then different algorithms of dimensionality reduction and clustering. The approach turned out to be very competitive for the Active Dict dataset, but didn't work well at all on the RuTenTen data.

## 2. Masked Language Modeling
In this notebook, I used DeepPavlov's vanilla RuBERT to obtain candidate words that are related to the target word by using special patterns containing the [MASK] token, constructed a TF-IDF matrix out of them and then tried clustering it. The approach produced much better results for the RuTenTen dataset, but was significantly less effective for the Active Dict data.

An important thing I observed during my experiments is that the RuTenTen data is, for some reason, incredibly sensitive to model hyperparameters.

The results of the experiments are all in their corresponding directories, so you are free to re-run the evaluation script to verify the obtained metrics.

Overall, I have invested a considerable amount of my free time into researching relevant papers, writing code and running innumerable experiments to achieve the best result possible in the short time that I had. I hope the contents are a useful testament to my skills in Natural Language Processing.
