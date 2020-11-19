---
layout: default
title: Backpropagation
permalink: /backpropagation.html
tags: categorisation neural-network deep-learning
---

[Cost function]({{site.url}}{{site.prod}}/cost-function.html),
[Forward propagation]({{site.url}}{{site.prod}}/forward-propagation.html)

### Definition

> "is that algorithm it can discover the optimal weights relatively quickly, even for a network with millions of weights."

> "Backpropagation tracks the derivatives of the activation functions in each successive neuron, 
>  to find weights that brings the loss function to a minimum, which will generate the best prediction. 
>  This is a mathematical process called [gradient descent]({{site.url}}{{site.prod}}/optimizers.html)."


### How backpropagation works [^2]


- After [forward propagation]({{site.url}}{{site.prod}}/forward-propagation.html) we get an output value which is the predicted value. 
- To calculate error we compare the predicted value with the actual output value. 
- We use a [loss function]({{site.url}}{{site.prod}}/cost-function.html) to calculate the error value. 
- Then we calculate the derivative of the error value with respect to each and every weight in the neural network. 
- Back-Propagation uses chain rule of Differential Calculus. 
- In chain rule first we calculate the derivatives of error value with respect to the weight values of the last layer. 
- We call these derivatives, [gradients]({{site.url}}{{site.prod}}/optimizers.html) and use these gradient values to calculate the gradients of the second last layer. 
- We repeat this process until we get gradients for each and every weight in our neural network. 
- Then we subtract this gradient value from the weight value to reduce the error value. 
- In this way we move closer (descent) to the Local Minima(means minimum loss).


#### Forward pass

- weights are initialized [^1]
- inputs **from the training set** are fed into the network [^1]
- The forward pass is carried out and the model generates its initial prediction[^1]

#### Cost function

- the error function is computed by checking how far away the prediction is from the known true value.[^1]

#### Gradient descent

- the backpropagation algorithm calculates how much the output values are affected by each of the weights in the model. 
To do this, it calculates partial derivatives, going back from the error function to a specific neuron and its weight. 
This provides complete traceability from total errors, back to a specific weight which contributed to that error. 
The result of backpropagation is a set of weights that minimize the error function.[^1]

#### Weights update

- weights can be updated after every sample in the training set, but this is usually not practical. 
Typically, a batch of samples runs in one big forward pass, and then backpropagation is performed on the aggregate result. 
The batch size and number of batches used in training, called iterations, are important hyperparameters that are tuned to get the best results. 
Running the entire training set through the backpropagation process is called an epoch.[^1]


<hr />

##### Footnotes:

[^1]: [missinglink.ai](https://missinglink.ai/guides/neural-network-concepts/complete-guide-artificial-neural-networks/)
[^2]: [missinglink.ai](https://hackernoon.com/everything-you-need-to-know-about-neural-networks-8988c3ee4491)
