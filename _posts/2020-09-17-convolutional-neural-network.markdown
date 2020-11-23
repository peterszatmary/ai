---
layout: default
title: Convolutional Neural Network
permalink: /convolutional-neural-network.html
tags: categorisation machine-learning technique neural-network deep-learning
---

[Machine learning]({{site.url}}{{site.prod}}/machine-learning.html),
[Recurrent Neural Networks (RNN)]({{site.url}}{{site.prod}}/recurrent-neural-network.html),
[Generative Adversarial Network (GAN)]({{site.url}}{{site.prod}}/generative-adversarial-network.html) 

### Definition

> "In deep learning, a convolutional neural network (CNN, or ConvNet) is a class of deep neural networks, most commonly
> applied to analyzing visual imagery. They are also known as shift invariant or space 
> invariant artificial neural networks (SIANN), based on their shared-weights architecture
> and translation invariance characteristics." [^3] 

### Architecture

It is one of the advanced Neural Network architectures

#### Other architectures

- [Recurrent Neural Networks (RNN)]({{site.url}}{{site.prod}}/recurrent-neural-network.html)
- [Generative Adversarial Network (GAN)]({{site.url}}{{site.prod}}/generative-adversarial-network.html) 
- [Capsule Neural network]({{site.url}}{{site.prod}}/capsule-neural-network.html)

### Is used

- in computer vision
- face recognition
- Identifying and classifying everyday objects in images
- Powering vision in robots and autonomous vehicles
- Recognizing scenes and suggest relevant captions
- Semantic parsing, sentence classification, and prediction
- Search query retrieval


### How it looks like

#### Layers

- Convolutional layer
- Activation layer (RELu layer)
- Pooling layer
- Fully connected layer

#### Layers description

- A CNN uses a three-dimensional structure, with three sets of neurons analyzing the three layers of a color image—red, green and blue.[^1]
- It analyzes an image one area at a time to identify important features [^1]
- **Convolution** In mathematics (in particular, functional analysis), convolution is a mathematical operation on two functions (f and g) 
that produces a third function (f∗g) that expresses how the shape of one is modified by the other.

Take a look on the picture

![CNN](/assets/images/cnn.png)

- first layer is **Convolution** which involves “scanning” the image, analyzing a small 
part of it each time, and creating a feature map with probabilities that each feature belongs to the required class.
First and second layer / steps are not fully connected because it would be than highly intensive and inefficient computation.
Instead of it fully connected layers come to the game later once there is smaller number of neurons[^1]
- The second step is [pooling]({{site.url}}{{site.prod}}/pooling.html), which reduces the dimensionality of each feature while maintaining its most important information. [^1]
- CNN can perform several rounds of convolution then pooling.
- Finally, when the features are at the right level of granularity, it creates a fully-connected neural network that analyzes the final probabilities and decides which class 
the image belongs to. The final step can also be used for more complex tasks, such as generating a caption for the image.[^1]
- Layers contains **filters** (matrices) one layer can have N matrices in size NxM.
- Filter definition : In signal processing, a filter is a device or process that removes some unwanted components or features from a signal.[^5]

### Pattern recognition with filters

![Pattern recognition with filters](/assets/images/pattern-recognition.jpeg)


<hr />

##### Footnotes:

[^1]: [Complete guide artificial neural networks](https://missinglink.ai/guides/neural-network-concepts/complete-guide-artificial-neural-networks/)
[^2]: [Convolutional neural network build one keras pytorch](https://missinglink.ai/guides/neural-network-concepts/convolutional-neural-network-build-one-keras-pytorch/)
[^3]: [Wikipedia CNN](https://en.wikipedia.org/wiki/Convolutional_neural_network)
[^4]: [Wikipedia Convolution](https://en.wikipedia.org/wiki/Convolution)
[^5]: [Wikipedia Filters](https://en.wikipedia.org/wiki/Filter_(signal_processing))
[^6]: [Tensorflow and CNN](https://missinglink.ai/guides/tensorflow/building-convolutional-neural-networks-tensorflow-three-examples/)