---
layout: default
title: Overfitting
permalink: /underfitting.html
tags: categorisation neural-network deep-learning training
---
 
[Overfitting]({{site.url}}{{site.prod}}/overfitting.html),
[backpropagation]({{site.url}}{{site.prod}}/backpropagation.html)
  
> "Happens when the neural network is good at learning its training set, but is not able to generalize its predictions to additional, unseen examples."
  
- in the other word we can say that our neural network is overtrained.
 
### Variance and Bias
 
- This is characterized by low bias and high variance. See bellow picture.
 
 
![bias]({{site.url}}{{site.prod}}/assets/images/bias-variance.png)
 
 
### Methods to avoid overfitting [^1]
 
- **Retraining neural networks** running the same model on the same training set but with different initial weights, and selecting the network with the best performance.
- **Multiple neural networks** training several neural network models in parallel, with the same structure but different weights, and averaging their outputs.
- **Early stopping** training the network, monitoring the error on the validation set after each iteration, and stopping training when the network starts to overfit the data.
- **Regularization** adding a term to the error function equation, intended to decrease the weights and biases, smooth outputs and make the network less likely to overfit.
- **Tuning performance ratio** similar to regularization, but using a parameter that defines by how much the network should be regularized.

##### Footnotes:
  
 [^1]: [missinglink.ai](https://missinglink.ai/guides/neural-network-concepts/complete-guide-artificial-neural-networks/)