# Micrograd
According to Micrograd's founder, **Andrej Karpathy**, MicroGrad is a tiny Autograd engine. Implements backpropagation (reverse-mode autodiff) over a dynamically constructed DAG and a small neural networks library with a PyTorch-like API on top of it. It consists of approximately 100 and 50 lines of code. The DAG only operates on scalar values, so each neuron is broken down into its individual additions and multiplications. However, as demonstrated in the demo notebook, this is sufficient to construct entire deep neural networks for binary classification. Possibly applicable for educational purposes.



Backpropagation is the algorithm that, according to Andrej Karpathy, enables one to effectively evaluates the **gradient of a loss function with respect to a neural network's weight**. It then enables us to i**teratively tune the weights of the neural network** to **minimise the loss function and increase the network's accuracy**.

As a result, Andrej Karpathy concludes that Backpropagation is the **mathematical core** of any c**ontemporary deep neural network** library.


## What exactly is backpropagation?

Backpropagation is used to adjust how accurately or precisely a neural network processes certain inputs. Backpropagation as a technique uses gradient descent: It calculates the gradient of the loss function at output, and distributes it back through the layers of a deep neural network.

