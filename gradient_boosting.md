# Gradient Boosting Algorithm for Machine Learning

Gradient Boosting is a powerful technique for building Predictive Models. Boosting algorithms work by weighting the observations, putting more weight on difficult to classify instances and less on those already handled well. New weak learners are added sequentially that focus their training on the more difficult patterns.

Thus boosting is a numerical optimization problem where the objective is to minimize the loss of the model by adding weak learners using a gradient descent like procedure. This class of algorithms is described as stage-wise additive model. This is because one new weak learner is added at a time and existing weak learners in the model and frozen and left unchanged.

The algorithm allows arbitrary differentiable loss functions to be used, expanding it to techniques beyond binary classification problems to support regression, multi-class classifications and more.

The Gradient Boosting Algorithm consists of mainly 3 parts:
1. a loss function to be optimized
2. a weak learner to make predictions
3. an additive model to add weak learners to minimize loss function

<img src="https://github.com/jpuri/deep-learning/blob/main/img/gradient_boosting.jpeg?raw=true" width="400px" alt="Gradient Boosting Algorithm">


