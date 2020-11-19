---
layout: default
title: Optimizers
permalink: /optimizers.html
tags: categorisation neural-network deep-learning training backpropagation
---

TODO

[backpropagation]({{site.url}}{{site.prod}}/backpropagation.html),
[Hyperparameters]({{site.url}}{{site.prod}}/hyperparameters.html)

### Gradient descent

- is an optimization algorithm to minimize [cost function]({{site.url}}{{site.prod}}/cost-function.html). (Minimize errors).
- Is finding local ,global minima of a function to determine the direction the mode should take to reduce errors.

#### Batch gradient descent

- computing the entire dataset.
- it takes time

#### Mini batch gradient descent

TODO

#### Stochastic gradient descent

- is computing on one sample data input.
- it converge much faster because it updates weights more frequently

### Gradient problems

Gradient problem lead to long training times, poor performance and low accuracy.

#### Vanishing gradient

- when the slope training is too small it is difficult to train.

#### Exploding gradient

- slope grow exponentially. 

### Gradient descent optimalization

TODO

##### Footnotes:

[^1]: [ruder.io](https://ruder.io/optimizing-gradient-descent/)
[^2]: [towardsdatascience.com](https://towardsdatascience.com/optimizers-for-training-neural-network-59450d71caf6)
[^3]: [An overview of gradient descent optimization algorithms](https://arxiv.org/pdf/1609.04747.pdf)
