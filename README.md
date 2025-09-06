# transformer-notebook

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/segusantos/transformer-notebook/blob/main/transformer.ipynb)

Decoder-only transformer implemented from scratch in [PyTorch](https://pytorch.org/) based on Andrej Karpathy's [nanoGPT lecture](https://youtu.be/kCc8FmEb1nY?si=mNj4qOlVlpTBxQ6E).

The model works on a per-character basis. Hence, the vocabulary is the set of all characters in the training data and no tokenization techniques are used.

The transformer can be trained on small texts and be used to generate sequences with a similar style, structure and in the same language as the training data. Due to the small size of the model, the generated text is mostly incoherent, though feel free to experiment with scaling the model size, training on larger datasets and using more complex tokenization policies.

The notebook can be easily executed locally if a GPU is available. Otherwise, it can be run on Google Colab with a GPU runtime. In case you wish to skip the training process, trained models for the datasets `martin_fierro.txt` and `shakespeare.txt` are provided.