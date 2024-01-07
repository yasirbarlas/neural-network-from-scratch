# INM702: Programming and Mathematics for Artificial Intelligence

Note: This repository and its contents support the coursework of the INM702 module at City, University of London.

We provide the code for Task 1 and Task 2, as Jupyter Notebooks. In Task 1 we create a neural network from scratch, and train it on the MNIST dataset. In Task 2, we use PyTorch to train a neural network on a London weather dataset. The output of the code is reproducible using the seed set in each notebook (which is 50).

## Task 1

Found in the 'task_1' folder.

Task 1 involves the creation of a neural network using only mathematical packages such as NumPy. We create a neural network class, that takes the input size, output size, number of hidden layers (and their nodes), activation function as parameters. Dropout regularisation and L1/L2 regularisation can be applied if desired.

We investigate the use of different architectures and parameters, and see how these changes can improve (or reduce) the test set accuracy. This can include the use of dropout regularisation, multiple hidden layers, and changes in activation function. We provide four optimisers that can be used, namely Batch Gradient Descent, Stochastic Gradient Descent, Mini-Batch Gradient Descent, and Adam.

NumPy Version == 1.24.3

## Task 2

Found in the 'task_2' folder.

Task 2 involves the use of PyTorch to create a recurrent neural network that can forecast daily mean temperatures. The dataset is from a weather station near Heathrow Airport in London, UK.

We investigate the use of different architectures and parameters, and see how these changes can improve (or reduce) the test set accuracy. Our base model uses an Long Short-Term Memory (LSTM) network with an additional Dense layer, using the Softmax activation function. The root-mean-squared propagation optimiser was used for the base model. We update the LSTM network to instead use the ReLU activation function, with the Adam optimiser. The different parameters that were changed include the use of dropout regularisation, multiple stacked LSTM layers, and multiple features in the hidden states.

PyTorch Version == 1.12.0+cpu
