---
layout: default
title: Multilayer perceptron
permalink: /multi-layer-perceptron.html
tags: categorisation neural-network deep-learning
---

[An activation function]({{site.url}}{{site.prod}}/activation-function.html)

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

At each neuron / perceptron in a hidden or output layer, the processing happens in two steps:

- **Preactivation** it is a weighted sum of inputs i.e. the linear transformation of weights to inputs available with added [bias]({{site.url}}{{site.prod}}/bias.html). 
**Based on this aggregated sum and activation function** the neuron makes a decision whether **to pass this information further or not**.
- **Activation** the calculated weighted sum of inputs is passed to the [activation function]({{site.url}}{{site.prod}}/activation-function.html).
Result of an activation function is output of perceptron and input for next layer perceptron. 

TODO calculations


![MLP]({{site.url}}{{site.prod}}/assets/images/perceptron-learning-process.png)




<hr />

##### Footnotes:

[^1]: [towardsdatascience.com](https://towardsdatascience.com/forward-propagation-in-neural-networks-simplified-math-and-code-version-bbcfef6f9250)