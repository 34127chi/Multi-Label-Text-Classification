# Deep Learning for Multi-Label Text Classification

This project is my research group project, and it is also a study of TensorFlow, Deep Learning(Fasttext, CNN, LSTM, RCNN, etc.).

The main objective of the project is to solve the multi-label text classification problem based on Convolutional Neural Networks. Thus, the format of the data label is like [0, 1, 0, ..., 1, 1] according to the characteristics of such problem.

## Requirements

- Python 3.6
- Tensorflow 1.8 +
- Numpy
- Gensim

## Data

Research data may attract copyright protection under China law. Thus, there is only code.

实验数据属于实验室与某公司的合作项目，涉及商业机密，在此不予提供，还望谅解。

## Innovation

### Data part
1. Make the data support **Chinese** and English.(Which use `jieba` seems easy)
2. Can use **your own pre-trained word vectors**.(Which use `gensim` seems easy)
3. Add embedding visualization based on the **tensorboard**.

### Model part
1. Add the correct **L2 loss** calculation operation.
2. Add **gradients clip** operation to prevent gradient explosion.
3. Add **learning rate decay** with exponential decay.
4. Add a new **Highway Layer**.(Which is useful based on the performance)
5. Add **Batch Normalization Layer**.

### Code part

1. Can choose to **train** the model directly or **restore** the model from checkpoint in `train.py`.
2. Can predict the labels via **threshold** and **topK** in `train.py` and `test.py`.
3. Add `test.py`, the **model test code**, it can show the predict value of each labels of the data in Testset when create the final prediction file.
4. Add other useful data preprocess functions in `data_helpers.py`.
5. Use `logging` for helping recording the whole info(including parameters display, model training info, etc.).

## Data Preprocessing

Depends on what your data and task are.

### Text Segment

You can use `jieba` package if you are going to deal with the chinese text data.

### Pre-trained Word Vectors

- Use `gensim` package to pre-train data.
- Use `glove` tools to pre-train data.
- Even can use a **fasttext** network to pre-train data.

## Network Structure

### FastText

![]()

References:

- [Bag of Tricks for Efficient Text Classification](https://arxiv.org/pdf/1607.01759.pdf)

---

### TextANN

![]()

References:

- **Personal ideas 🙃**

---


### TextCNN

![]()

References:

- [Convolutional Neural Networks for Sentence Classification](http://arxiv.org/abs/1408.5882)
- [A Sensitivity Analysis of (and Practitioners' Guide to) Convolutional Neural Networks for Sentence Classification](http://arxiv.org/abs/1510.03820)

---

### TextRNN

**Warning: Model can use but not finished yet 🤪!**

#### TODO
1. Add BN-LSTM cell unit.
2. Add attention.

![]()

References:

- [Recurrent Neural Network for Text Classification with Multi-Task Learning](http://www.aaai.org/ocs/index.php/AAAI/AAAI15/paper/download/9745/9552)

---

### TextRCNN

**Warning: Not finished yet 🤪!**

![]()

References:

- [Recurrent Convolutional Neural Networks for Text Classification](http://www.aaai.org/ocs/index.php/AAAI/AAAI15/paper/download/9745/9552)

---

### TextCRNN

![]()

References:

- **Personal ideas 🙃**

---

### TextHAN

![]()

References:

- [Hierarchical Attention Networks for Document Classification](https://www.cs.cmu.edu/~diyiy/docs/naacl16.pdf)

---

### TextSANN

**Warning: Model can use but not finished yet 🤪!**

#### TODO
1. Add attention penalization loss.
2. Add visualization.

![]()

References:
- [A STRUCTURED SELF-ATTENTIVE SENTENCE EMBEDDING](https://arxiv.org/pdf/1703.03130.pdf)

---

## About Me

黄威，Randolph

SCU SE Bachelor; USTC CS Master

Email: chinawolfman@hotmail.com

My Blog: [randolph.pro](http://randolph.pro)

LinkedIn: [randolph's linkedin](https://www.linkedin.com/in/randolph-%E9%BB%84%E5%A8%81/)
