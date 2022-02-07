# my_Neural_Network

In this notebook I would like to implement my first **Neural Network** from scratch.
To do so, I will apply it to the [MNIST database](https://en.wikipedia.org/wiki/MNIST_database): a large database of handwritten digits. We will predict if a given digit is a zero or not.

The main idea of [neural networks](https://en.wikipedia.org/wiki/Artificial_neural_network) is the following.
- We start with some random parameters W and b.
- Next, we implement the **forward propagation step**. This has several *layers*, each of which predicts an output
g (W * A + b),
where
A 
is the output of the previous layer and  g 
is the [*activation function*](https://en.wikipedia.org/wiki/Activation_function). 
Clearly, the input of the fist layer is an image of the dataset.
- We compute the *Cross-Entropy cost* of the final output: this tends to zero when we make correct predictions.
- At this point, our goal is to minimize the cost to make better predictions using **gradient descent**. To do so, we look for a minimum of the cost function by taking the derivatives of the cost function and "making a step towards the minimum" changing the parameters W and b. This is called the **backward propagation step**.
