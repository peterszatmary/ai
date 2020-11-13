---
layout: default
title: Multilayer perceptron
permalink: /multi-layer-perceptron.html
tags: categorisation neural-network deep-learning
---

TODO

### Definitions


#### Perceptron

> " is a binary classification algorithm modeled after the functioning of the human brain—it was intended to emulate 
> the neuron. The perceptron, while it has a simple structure, has the ability to learn and solve very complex problems."


![perceptron]({{site.url}}{{site.prod}}/assets/images/perceptron.png)

#### Multilayer perceptron (MLP)

> "is a group of perceptrons, organized in multiple layers, that can accurately answer complex questions. 
> Each perceptron in the first layer (on the left) sends signals to all the perceptrons in the second layer, and so on.
> An MLP contains an input layer, at least one hidden layer, and an output layer."


![MLP]({{site.url}}{{site.prod}}/assets/images/mlp.png)

#### Perceptron learning process

- Takes the inputs which are fed into the perceptrons in the input layer, multiplies them by their weights, and computes the sum.
- Adds the number one, multiplied by a “bias weight”. This is a technical step that makes it possible to move the output function of each perceptron (the activation function) up, down, left and right on the number graph.
- Feeds the sum through the activation function—in a simple perceptron system, the activation function is a step function.
The result of the step function is the output. 

![MLP]({{site.url}}{{site.prod}}/assets/images/perceptron-learning-process.png)

