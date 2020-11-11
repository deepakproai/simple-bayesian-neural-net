# A Simple Bayesian Neural Network

Usually, the parameters (weights and biases) of any deep learning model are fixed. These parameters are decided using iterative optimization techniques like gradient descent and it works quite well. Bayesian Neural Networks function differently, instead of learning a deterministic set of parameters, they learn a distribution of weights and biases for a given training set. So, what we do in practice is that we forward pass the input image multiple times with a new sample of model parameters every time, giving us a distribution of output values. We can use these set of outputs to determine how certain/uncertain the model is of its prediction.

This repository implements a simple Bayesian Neural Network on the MNIST dataset using Pyro which is a probabilistic programming framework built on top of PyTorch.

## Requirements
- Pyro
- PyTorch
- Torchvision
- Numpy

## Usage
You can easily run the notebook in this repository using Colab <a href="https://colab.research.google.com/github/nerdimite/simple-bayesian-neural-net/blob/master/Bayesian%20Neural%20Network.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/></a>

## References
- Pyro http://pyro.ai/examples/
- Variational Bayes and Beyond (ICML 2018 Tutorial) - https://www.youtube.com/watch?v=DYRK0-_K2UU
- https://towardsdatascience.com/making-your-neural-network-say-i-dont-know-bayesian-nns-using-pyro-and-pytorch-b1c24e6ab8cd