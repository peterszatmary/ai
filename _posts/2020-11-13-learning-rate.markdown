---
layout: default
title: Learning rate
permalink: /learning-rate.html
tags: categorisation neural-network deep-learning training hyperparameters
---

[Hyperparameters]({{site.url}}{{site.prod}}/hyperparameters.html),
[Cost function]({{site.url}}{{site.prod}}/cost-function.html)

### Definition

> "determines how quickly or how slowly you want to update your weight(parameter) values."

- Is one of [Hyperparameters]({{site.url}}{{site.prod}}/hyperparameters.html) used to train the model.

- When we train neural networks we usually use [Gradient Descent]({{site.url}}{{site.prod}}/optimizers.html) to optimize the weights. 
At each iteration we use [back-propagation]({{site.url}}{{site.prod}}/backpropagation.html) to calculate the derivative of the loss function with respect to each weight and subtract it from that weight. 
Learning rate determines how quickly or how slowly you want to update your weight(parameter) values. 
Learning rate should be high enough so that it won’t take ages to **converge**, and it should be low enough so that it finds the local minima.

###  Terminology used

- **Accuracy** refers to the closeness of a measured value to a standard or known value.
- **Precision** refers to the closeness of two or more measurements to each other. It is the repeatability or reproducibility of the measurement.
- **Recall(Sensitivity)** refers to the fraction of relevant instances that have been retrieved over the total amount of relevant instances.
- **Convergence** is when as the iterations proceed the output gets closer and closer to a specific value.
- **Regularization** It is used to overcome the [over-fitting problem]({{site.url}}{{site.prod}}/overfitting.html). 
In regularization we penalise our loss term by adding a L1 (LASSO) or an L2(Ridge) norm on the weight vector w (it is the vector of the learned parameters in the given algorithm).

![learning rate]({{site.url}}{{site.prod}}/assets/images/training/learning-rate.png)


### Possible problems

#### Learning rate to low 

- training of the model will progress very slowly as we are making minimal updates on weights.

#### Learning rate to high

- divergent behaviour to the [cost function]({{site.url}}{{site.prod}}/cost-function.html) because of drastic updates on weights.

<hr />

##### Footnotes:


