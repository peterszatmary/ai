---
layout: default
title: Activation function
permalink: /activation-function.html
tags: categorisation neural-network deep-learning hyperparameters
---

[Cost function]({{site.url}}{{site.prod}}/cost-function.html),
[Hyperparameters]({{site.url}}{{site.prod}}/hyperparameters.html)

### Definition

> "An activation function is a mathematical equation that determines the output of each element (perceptron or neuron) in the neural network. 
> It takes in the input from each neuron and transforms it into an output, usually between one and zero or between -1 and one."

### Activation of neuron

- is mathematically a function of its inputs.


### Activation functions

- also known as (Transfer Function)
- determine the output of a deep learning model, its accuracy, also the computational efficiency of training a model—which can make or break a large scale neural network. [^3]
- have a major effect on the neural network’s ability to converge and the convergence speed. [^3]
- When building a model and training a neural network, the selection of activation functions is critical. Experimenting with different activation functions for different problems will allow you to achieve much better results.
- are central to deep learning architectures
- decides whether neuron should be fired or not [^1]
- accepts the weighted sum of inputs, and a bias as input to any activation function [^1]
- *Y = sum ( weight * input ) + bias* [^1]
- the node which gets fired depends on the value Y [^1]
- must be computationally efficient [^3]
- Each neuron has a weight, and multiplying the input number with the weight gives the output of the neuron, which is transferred to the next layer.[^3]
- Increasingly, neural networks use non-linear activation functions[^3]
- Each neuron’s output is the input of the neurons in the next layer of the network, and so the inputs cascade through multiple activation functions until eventually, the output layer generates a prediction.

![Activation function]({{site.url}}{{site.prod}}/assets/images/activation-function/activation-fun.png)


### Activation function categories

- **Ridge activation functions** ( are univariate functions acting on a linear combination of the input variables. )[^2]
- **Radial activation functions** ( A special class of activation functions known as radial basis functions (RBFs) are used in RBF networks, which are extremely efficient as universal function approximators. These activation functions can take many forms )[^2]
- **Folding activation functions** ( Folding activation functions extensively used in the pooling layers in convolutional neural networks, and in output layers of multiclass classification networks. )[^2]

- **step function**
- **linear functions**
- **non linear functions**

#### Binary step

- CON: The problem with a step function is that it does not allow multi-value outputs—for example, it cannot support classifying the inputs into one of several categories.[^3]

[![sigmoid]({{site.url}}{{site.prod}}/assets/images/activation-function/step.png)](https://www.simplilearn.com/tutorials/deep-learning-tutorial/deep-learning-interview-questions)

- [Binary step]()

#### Linear functions

- It takes the inputs, multiplied by the weights for each neuron, and creates an output signal proportional to the input. [^3]
- PRO : is better than a step function because it allows multiple outputs, not just yes and no.[^3]
- CON : Not possible to use [backpropagation]({{site.url}}{{site.prod}}/backpropagation.html) (gradient descent) to train the model. The derivative of the function is a constant, and has no relation to the input, X.[^3]
- CON : All layers of the neural network collapse into one. the last layer will be a linear function of the first layer (because a linear combination of linear functions is still a linear function). So a linear activation function turns the neural network into just one layer.[^3]
- A neural network with a linear activation function is simply a linear regression model [^3]

#### Non linear functions

- They allow backpropagation because they have a derivative function which is related to the inputs.
- They allow “stacking” of multiple layers of neurons to create a deep neural network. Multiple hidden layers of neurons are needed to learn complex data sets with high levels of accuracy.

Next you can find some of them most popular ones.

##### Common Non linear functions

###### Sigmoid / Logistic

- has a smooth gradient and outputs values between zero and one. 
- For very high or low values of the input parameters, the network can be very slow to reach a prediction, called the vanishing gradient problem.

[![sigmoid]({{site.url}}{{site.prod}}/assets/images/activation-function/sigmoid.png)](https://www.simplilearn.com/tutorials/deep-learning-tutorial/deep-learning-interview-questions)

For more information see [Sigmoid](https://en.wikipedia.org/wiki/Sigmoid_function)



###### Tanh

- is zero-centered making it easier to model inputs that are strongly negative strongly positive or neutral.

[![tanh]({{site.url}}{{site.prod}}/assets/images/activation-function/tanh.png)](https://www.simplilearn.com/tutorials/deep-learning-tutorial/deep-learning-interview-questions)

- [Tanh]()

###### Rectified linear unit (ReLU)

- Is ridge activation function. 
- It is often used to activate hidden layers in neural networks. [^1]
- Results between 0 - 1 
- is highly computationally efficient but is not able to process inputs that approach zero or negative.

[![relu]({{site.url}}{{site.prod}}/assets/images/activation-function/relu.png)](https://www.simplilearn.com/tutorials/deep-learning-tutorial/deep-learning-interview-questions)

- [ReLU]({{site.url}}{{site.prod}}/rectified-linear-unit.html)

###### The Leaky ReLu

- function has a small positive slope in its negative area, enabling it to process zero or negative values.

TODO img

##### The Parametric ReLu

- function allows the negative slope to be learned, performing backpropagation to learn the most effective slope for zero and negative input values.

###### Softmax

- It is folding activation function. 
- It is often used to activate output layers in neural networks. [^1]
- It normalizes outputs for each class between 0 and 1, and returns the probability that the input belongs to a specific class.

- [Softmax]({{site.url}}{{site.prod}}/softmax.html)

##### Swish

- is a new activation function discovered by Google researchers. [^4]
- It performs better than ReLu with a similar level of computational efficiency.[^4]
- In 2017, after performing analysis on ImageNet data, researchers from Google alleged that using the function as an activation function in artificial neural networks improves the performance, compared to ReLU and sigmoid functions.[^4]
- It is believed that one reason for the improvement is that the swish function helps alleviate the vanishing gradient problem during backpropagation.[^4]


####



#### Future

[Recent research by Franco Manessi and Alessandro Rozza](https://arxiv.org/pdf/1801.09403.pdf) attempted to find ways to automatically learn which is the 
optimal activation function for a certain neural network and to even automatically combine activation functions to achieve
 the highest accuracy. This is a very promising field of research because it attempts to discover an optimal activation 
 function configuration automatically, whereas today, this parameter is manually tuned.

<hr />

##### Footnotes:

[^1]: [simplilearn.com](https://www.simplilearn.com/tutorials/deep-learning-tutorial/deep-learning-interview-questions)
[^2]: [Wikipedia activation function](https://en.wikipedia.org/wiki/Activation_function)
[^3]: [missinglink.ai](https://missinglink.ai/guides/neural-network-concepts/7-types-neural-network-activation-functions-right/)
[^4]: [Wikipedia swish](https://en.wikipedia.org/wiki/Swish_function)
[^5]: [towardsdatascience.com](https://towardsdatascience.com/forward-propagation-in-neural-networks-simplified-math-and-code-version-bbcfef6f9250)
