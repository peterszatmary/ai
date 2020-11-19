---
layout: default
title: Underfitting
permalink: /underfitting.html
tags: categorisation neural-network deep-learning training
---

[Overfitting]({{site.url}}{{site.prod}}/overfitting.html),
[backpropagation]({{site.url}}{{site.prod}}/backpropagation.html)
 
> "Happens when the neural network is not able to accurately predict for the training set, not to mention for the validation set."
 
- in the other word we can say that our neural network is undertrained.

### Variance and Bias

- This is characterized by high bias and high variance. See bellow picture.


![bias]({{site.url}}{{site.prod}}/assets/images/bias-variance.png)


### Methods to avoid underfitting [^1]

- **Adding neuron layers or inputs** adding neuron layers, or increasing the number of inputs and neurons in each layer,
 can generate more complex predictions and improve the fit of the model.
- **Adding more training samples or improving quality** the more training samples you feed into the network, 
and the better they represent the variance in the real population, the better the network will perform.
- **Dropout** randomly “kill” a certain percentage of neurons in every training iteration. 
This ensures some information learned is randomly removed, reducing the risk of overfitting.
- **Decreasing regularization parameter** regularization can be overdone. By using a regularization performance parameter,
 you can learn the optimal degree of regularization, which can help the model better fit the data.


##### Footnotes:
 
[^1]: [missinglink.ai](https://missinglink.ai/guides/neural-network-concepts/complete-guide-artificial-neural-networks/)