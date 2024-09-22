# What is Neural Network ?

Neural Networks as the name suggest is network of neurons. This structure actually resembles the network os neurons in brain. Neurons are predictors, they map an input X to an output Y. The output of one neuron is input for the next.

![Deep Neural Network](https://github.com/jpuri/deep-learning/blob/main/img/neural_network.png?raw=true)

<img src="https://github.com/jpuri/deep-learning/blob/main/img/neural_network.png?raw=true" width="200px" alt="Deep Neural Network">

Neural networks have multiple layers of neurons comprising of an input, output and hidden layers in the middle. Each layer can be imagined as a stack of neurons placed on top of each other.

# Liner Regression Model of Neurons

Each neuron is in itself a liner regression model. In vectorised notation it can be represented as:

```
Y = WX + b
```

Thus each neuron has:

1. Input vector `X`
2. Weight `W`
3. Bias `b`
4. Output `Y`

The weight helps to determine the importance of the input parameter. You can imagine Neural Network as a mesh of these Linear Regression Models where output of one is input for the next. Additionally in Neural Network an activation function is applied to the output of Linear Regression Model.

# Activation Function

Activation functions transform the input signal of a node in a neural network into an output signal that is then passed on to the next layer. Activation functions introduce non-linearities, allowing neural networks to learn highly complex mappings between inputs and outputs. Choosing the right activation function is crucial for training neural networks that generalize well and provide accurate predictions.

Types of Activation Functions
Neural networks leverage various types of activation functions, each activation function has its own unique properties and is suitable for certain use cases. 

    - Linear activation
    - Sigmoid activation
    - Tanh (hyperbolic tangent) activation
    - ReLU (rectified linear unit) activation
    - Softmax activation

# Deep Learning

The process of training neural networks is known as Deep Learning.

When neural neworks are implemented they are trained by giving then training data set of inputs mapping to output. Thus given `X` and `Y` neural networks are very good at determining the rest of paremeters. They are able to comprehend un-structured data and identify non-linear and complex relationship between data points. This is also known as supervised learning.

Actual neural networks may have even millions of there tiny neurons. Once trained neural networks are very effective in predicting the mapping of an input parameter to an output. It is an adaptive system that improves continuously, and neural networks are able to solve complicated problems with greater accuracy.

# Use Cases

Neural Networks have several use cases across various indistries, these can be broadly classified as:

1. Computer vision
With neural networks, computers can distinguish and recognize images similar to humans. Computer vision has several applications, such as the following:

    - Visual recognition in self-driving cars
    - Content moderation to automatically remove unsafe or inappropriate content
    - Facial recognition

2. Speech recognition
Neural networks can analyze human speech despite varying speech patterns, pitch, tone, language, and accent.

    - Assist call center agents
    - Convert clinical conversations into documentation
    - Accurately subtitle videos and meeting recordings

3. Natural language processing
Neural networks help computers gather insights and meaning from text data and documents. NLP has several use cases, including in these functions:

    - Automated virtual agents and chatbots
    - Automatic organization and classification of written data
    - Business intelligence analysis of long-form documents like emails and forms
    - Indexing of key phrases
    - Document summarization and article generation

Recommendation engines
Neural networks can track user activity to develop personalized recommendations. They can also analyze all user behavior and discover new products or services that interest a specific user.