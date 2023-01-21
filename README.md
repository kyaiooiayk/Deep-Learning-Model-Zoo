# Deep-Learning-Model-Zoo
References for deep learning models implemented in TensorFlow or PyTorch. The inspiration for this repository was taken from this [repository](https://github.com/rasbt/deeplearning-models). This repository will try to build on this and provide a concise extra references following a common template. For each **deep learning model** the following reference template is provided":
  - TensorFlow 1/2 implementation. See [this](https://www.tensorflow.org/guide/migrate) taken directly from the tensorflow website inhow you can migrate from TF1 to TF2. Alternatively you can use this nice [app](http://tf2up.ml/)
  - PyTorch implementation
  - Original paper
  - Any other useful references
***

## TF1 vs. TF2
- [How to migrate from TensorFlow 1.x to TensorFlow 2](https://www.tensorflow.org/guide/migrate)
- [Tensorflow 1.x to Tensorflow 2.0 — Coding changes](https://medium.com/red-buffer/tensorflow-1-0-to-tensorflow-2-0-coding-changes-636b49a604b)
- [Series of questions on TF vs. PT](https://cementanswers.com/is-tensorflow-2-backward-compatible/)
- [How to resolve: AttributeError: module ‘tensorflow’ has no attribute ‘placeholder’ ](https://gimoonnam.github.io/machinelearning/tensorFlow_1/). 
- Quick answer #1:
```
# Tensorflow 1.x
self._states = tf.placeholder(shape=[None, self._num_states], dtype=tf.float32)
# Tensorflow 2.x
self._states = tf.Variable(tf.ones(shape=[None, self._num_states]), dtype=tf.float32)
```
- Quick answer #2:
```
import tensorflow.compat.v1 as tf
tf.disable_v2_behavior()
x = tf.placeholder(shape=[None, 2], dtype=tf.float32)
```
***

## Traditional ML models

- **Perceptron**<br/>
  [
  [TensorFlow1](https://github.com/rasbt/deeplearning-models/blob/master/tensorflow1_ipynb/basic-ml/perceptron.ipynb) | 
  [PyTorch](https://github.com/rasbt/deeplearning-models/blob/master/pytorch_ipynb/basic-ml/perceptron.ipynb) |
  [Wiki](https://en.wikipedia.org/wiki/Perceptron)
  ]

- **Logitic Regression**<br/>
  [
  [TensorFlow1](https://github.com/rasbt/deeplearning-models/blob/master/tensorflow1_ipynb/basic-ml/logistic-regression.ipynb) |
  [PyTorch](https://github.com/rasbt/deeplearning-models/blob/master/pytorch_ipynb/basic-ml/logistic-regression.ipynb)
  ]

- **Vanilla MLP (Multi-Layer Perceptrons)**<br/>
  [
  [TensorFlow1](https://github.com/rasbt/deeplearning-models/blob/master/tensorflow1_ipynb/mlp/mlp-basic.ipynb) |
  [PyTorch](https://github.com/rasbt/deeplearning-models/blob/master/pytorch_ipynb/mlp/mlp-basic.ipynb)
  ]
  
- **MLP with dropout**<br/>
  [
  [TensorFlow1](https://github.com/rasbt/deeplearning-models/blob/master/tensorflow1_ipynb/mlp/mlp-dropout.ipynb) |
  [PyTorch](https://github.com/rasbt/deeplearning-models/blob/master/pytorch_ipynb/mlp/mlp-dropout.ipynb)
  ]
  
- **MLP with batch normalisation**<br/>
  [
  [TensorFlow1](https://github.com/rasbt/deeplearning-models/blob/master/tensorflow1_ipynb/mlp/mlp-batchnorm.ipynb) |
  [PyTorch](https://github.com/rasbt/deeplearning-models/blob/master/pytorch_ipynb/mlp/mlp-batchnorm.ipynb)
  ]
***

## Everything else

- **Cycle GAN**
[
[PyTorch](https://github.com/theopfr/cycle-gan-pytorch) | [Paper](https://arxiv.org/abs/1703.10593)
]

## Template
- **Template**<br/>
  [
  TensorFlow1 |
  TensorFlow2 |
  PyTorch
  ]
  
***
