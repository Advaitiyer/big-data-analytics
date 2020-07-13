**Task 1: Multi-layer Perceptron**

This task is to choose the best model based on accuracy between multilayer perceptrons predicting whether a face is from an old person or not based on pixels. 

The comparison is conducted between:

- No hidden layers
- One hidden layer with 10 neurons
- Two hidden layers with 30 neurons each

Both models are fit to training and estimate the AUC on validation. You don't need to build a pipeline because the features needed are in the column pixels. Pick the best one based on validation performance. The input dimension is 2304 (=48x48) and the output is 2. Store the first, second, and third models in the variables mlp_model1, mlp_model2, and mlp_model3. Additionally, fit a logistic regression model and call it lr_model. Store the AUC on AUC1, AUC2, AUC3, and AUC_lr. Based on these performances, store the best model in best_model. Use the default paramerts for all the neural networks.

**Task 2: Convolutional Neural Network**

This task is meant to analyze different architectures for the prediction of MNIST digits. 

**Data Loading and Flattening**

This step loads the MNIST data and creates a data loader for training and testing (trainloader and testloader, respectively). Also, it defines a special layer that flattens a volumetric layer into a set of neurons (Flatten) leaving the road ready for creating a fully connected layer.

**Convolution**

The function create_cnn creates a very specific architecture (CONV => ReLU => MaxPool => FC). Consider that the MNIST images have width and height 28. The convolutional layer has a 3 kernels of size 4, stride of 2, and padding of 2. The max pooling layer has a kernel size of 3 and stride of 2.

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/Week6.png?raw=true"/>


