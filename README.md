# Alphabet_Recognition
During our experiments, we created two models (model 1, model 2) with different architectures, where we applied the convolutional neural network architecture on the model and the multi
-layered Perceptron architecture on model 2 In what follows we present the architecture of the two models:
## CNNs Architecture 
The first model of CNNs is composed of two layers of convolution and one layer of max pooling and two layers of fully connected.
The input image is 26 * 26, the image goes to the first convolution layer first. This layer is composed of 32 filters of size 3 * 3, Each of our convolution layers is followed by an activation function ReLu this function forces the neurons to return positive values, after this convolution 32 feature maps of size 26 * 26 will be created.
The 32 feature maps are given at the input of the second convolution layer which is also composed of 64 filters, a RELU activation function is applied on the convolution layer, then Max Pooling is applied to reduce the size of the image thus the quantity of parameters and calculation. At the end of this layer, we will have 32 feature maps of size 12 * 12.

After these two layers of convolution, we use a neural network composed of two fully connected layers. The first has a 128 neurons where the activation function used is the ReLU, and the second is a softmax which allows to calculate the probability distribution of the 26 classes 
(the number of classes in the image base of the set of EMNIST data).

## MLP Architecture 
The second model that we present ( MLP ) is composed of three fully connected layers. The two each have 512 neurons where the activation function used is the rereader and the third layer is a softmax which allows to calculate the probability distribution of the 26 classes (the number of class in the image base of the set of EMNIST data)

## Results
We have achieved an accuracy of 90% for the MPL model & 91 for the CNNs model
