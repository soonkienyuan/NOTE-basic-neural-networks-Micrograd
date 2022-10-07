# Discover Micrograd - backpropagation and neural network training

End to End Note for backpropagation and neural network training of the Micrograd.

## Introduction

According to Micrograd's founder, **Andrej Karpathy**, MicroGrad is a tiny Autograd engine. Implements backpropagation (reverse-mode autodiff) over a dynamically constructed DAG and a small neural networks library with a PyTorch-like API on top of it. It consists of approximately 100 and 50 lines of code. The DAG only operates on scalar values, so each neuron is broken down into its individual additions and multiplications. However, as demonstrated in the demo notebook, this is sufficient to construct entire deep neural networks for binary classification. Possibly applicable for educational purposes.



Backpropagation is the algorithm that, according to Andrej Karpathy, enables one to effectively evaluates the **gradient of a loss function with respect to a neural network's weight**. It then enables us to i**teratively tune the weights of the neural network** to **minimise the loss function and increase the network's accuracy**.

As a result, Andrej Karpathy concludes that Backpropagation is the **mathematical core** of any c**ontemporary deep neural network** library.


## What exactly is backpropagation?

Backpropagation is used to adjust how accurately or precisely a neural network processes certain inputs. Backpropagation as a technique uses gradient descent: It calculates the gradient of the loss function at output, and distributes it back through the layers of a deep neural network.

## Summary
- Neural network are the simple mathematics expression in the case of multi-layer perceptron that take input as the data and weight

- The parameters of the neural network mathematics expression for the forward pass followed by a loss function.

- The loss function try to measure the accuracy of the predictions and usually the loss will be low as your prediction matching your target or the network behaving well

- We manipulate the loss function so that when the loss function is low, the network is doing what you want it to do on your problem

- We backward the loss and use backpropagation to get the gradient and then we know how to tune all the parameters to decrease the loss locally. Then we need to iterate the process many times in what's called the gradient descent

- Minimize the loss based on the gradient information.
