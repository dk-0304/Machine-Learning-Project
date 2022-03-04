# Machine-Learning-Project

## Purpose

This is to Identify images using the TensorFlow Library. Essenntially, the library already has a store of differet image libraries ad in this case photos of flowers are used. The code then creates a model to train and identify the objects in the images. Ultimately it displays the results of the training and the accuracy in the form of graphs.

### Type of Model

TensorFlow uses a sequential model which is used for a plain stack of layers where each layer has exactly one input tensor and one output tensor.

## Does it use Supervised Learning?

Supervised learning *uses labeled datasets to train algorithms* to classify data or predict outcomes accurately. The algorithm measures its accuracy through the loss function, adjusting until the error has been sufficiently minimized. In this case, *yes this model is using supervised learning* by feeding hundreds of photos of different kinds of flowers including dandelions, roses, sunflowers, etc.

Running my program does show this training:

> Epoch 1/10
> 92/92 [==============================] - 3s 16ms/step - loss: 1.2769 - accuracy: 0.4489 - val_loss: 1.0457 - val_accuracy: 0.5804

> Epoch 2/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.9386 - accuracy: 0.6328 - val_loss: 0.9665 - val_accuracy: 0.6158

> Epoch 3/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.7390 - accuracy: 0.7200 - val_loss: 0.8768 - val_accuracy: 0.6540

> Epoch 4/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.5649 - accuracy: 0.7963 - val_loss: 0.9258 - val_accuracy: 0.6540

> Epoch 5/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.3662 - accuracy: 0.8733 - val_loss: 1.1734 - val_accuracy: 0.6267

> Epoch 6/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.2169 - accuracy: 0.9343 - val_loss: 1.3728 - val_accuracy: 0.6499

> Epoch 7/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.1191 - accuracy: 0.9629 - val_loss: 1.3791 - val_accuracy: 0.6471

> Epoch 8/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.0497 - accuracy: 0.9871 - val_loss: 1.8002 - val_accuracy: 0.6390

> Epoch 9/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.0372 - accuracy: 0.9922 - val_loss: 1.8545 - val_accuracy: 0.6390

> Epoch 10/10
> 92/92 [==============================] - 1s 11ms/step - loss: 0.0715 - accuracy: 0.9813 - val_loss: 2.0656 - val_accuracy: 0.6049

## Results

![results](https://www.tensorflow.org/tutorials/images/classification_files/output_jWnopEChMMCn_0.png#gh-light-mode-only)

The plots show that training accuracy and validation accuracy are off by large margins, and the model has achieved only around 60% accuracy on the validation set.

## Back Propogation and Artificial Neural Nets

This program does use artificial neural nets and I believe the graph shows the back propogatio through the loss diagram as tensorflow has an auto gradient feature. Back propogation basically is the algorithm used along with an optimization algorithm such as Gradient Descent (GD) to learn the parameters of a NN model. BP produces gradients which are then used in optimization. *_[Useful Link to understand BP](https://towardsdatascience.com/error-backpropagation-5394d33ff49b)_*

![image](https://user-images.githubusercontent.com/96376049/156680565-71ac65aa-d5df-4e37-9aff-100d7d338b9c.png)

The purpose of an artificial neural network is to mimic how the human brain works with the hope that we can build a machine that behaves like a human. Artificial neural networks (ANNs) are comprised of a node layers, containing an input layer, one or more hidden layers, and an output layer. Each node, or artificial neuron, connects to another and has an associated weight and threshold. If the output of any individual node is above the specified threshold value, that node is activated, sending data to the next layer of the network. Otherwise, no data is passed along to the next layer of the network. *_[IBM Link all about neural networks](https://www.ibm.com/cloud/learn/neural-networks)_*

![Back Prpogation Diagram](https://www.tensorflow.org/tutorials/images/classification_files/output_dduoLfKsZVIA_0.png)

## Reinforcement Learning

In reinforcement learning, developers devise a method of rewarding desired behaviors and punishing negative behaviors. This method assigns positive values to the desired actions to encourage the agent and negative values to undesired behaviors.

This code could be changed to add a score counter maybe and negative marking for every image that has been processed correctly or not.

## Clustering, Regression, or Classification

### Clustering

![image](https://user-images.githubusercontent.com/96376049/156692462-79055751-f5ab-432e-b1f2-e1b05e4317e7.png)

Clustering means grouping data based onn similar charactersitics and this would not be viable for this algorithm as the model is based onn ulabelled data and unsupervised learing however, this code is based o supervised learning. To adapt Ibelieve I would have to remove the labels and add some more parameters to group large groups of data.

### Regression

![image](https://user-images.githubusercontent.com/96376049/156692504-6b123a59-8030-41b8-90e8-d21fb22cf7b5.png)

Regression analysis consists of a set of machine learning methods that allow us to predict a continuous outcome variable (y) based on the value of one or multiple predictor variables (x). Briefly, the goal of regression model is to build a mathematical equation that defines y as a function of the x variables.

Since this works with cotinuous data types such as price or length that can actually be turnned into a mathematical equation, this code can't be using one as it is based on images. To adapt i would have to change the entoire basis of what the program is trying to lern and make it measurable with a correlation.

### Classification

I believe this program IS using classification as data is passed already labelled innto the different types of flowers and the program is learning to identify each category of flowers.
