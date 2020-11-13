---
layout: default
title: Deep neural network
permalink: /deep-neural-network.html
tags: categorisation neural-network deep-learning
---

[Cost function]({{site.url}}{{site.prod}}/cost-function.html)

### Definition

> "Artificial Neural Networks (ANN) is a supervised learning system built of a large number of simple elements, called 
> neurons or perceptrons. Each neuron can make simple decisions, and feeds those decisions to other neurons, organized 
> in interconnected layers. Together, the neural network can emulate almost any function, and answer practically any
> question, given enough training samples and computing power."

### Neural network 

- consist of input layer, output layer and one hidden layer. Layers contain nodes with edges.

![Non deep NN]({{site.url}}{{site.prod}}/assets/images/deep/non-deep.png)

### Deep Neural network 

- is the same structure consisting from one input layer, one output layer but more than one hidden layer ( 2 - 8 ).
- Research from Goodfellow, Bengio and Courville and other experts suggests that neural networks increase in accuracy with the number of hidden layers [^3]

![Non deep NN]({{site.url}}{{site.prod}}/assets/images/deep/deep.png)

### From Perceptron to Deep Neural Network

A multilayer perceptron is quite similar to a modern neural network. By adding a few ingredients, the perceptron 
architecture becomes a full-fledged deep learning system:

- activation function
- backpropagation
- advanced architectures : CNN, RNN, GAN.

<hr />

##### Footnotes:

[^3]: [missinglink.ai](https://missinglink.ai/guides/neural-network-concepts/7-types-neural-network-activation-functions-right/)
