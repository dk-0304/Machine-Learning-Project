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
