
# DCGAN Implementation

## Introduction
We have used an existing [Deep Convolutional Generative Adversarial Networks repo](https://github.com/awjuliani/TF-Tutorials/blob/master/DCGAN.ipynb) to train the MNIST database to understand the working/ architecture of standard GAN.

## Requirements

* Tensorflow 1.1
* Tensorflow slim library
* MNIST dataset


## Network

# Generator
The generator takes a vector of random numbers and transforms it into a 32x32 image. Each layer in the network involves a strided transpose convolution, batch normalization, and rectified nonlinearity. Tensorflow's slim library allows us to easily define each of these layers.

# Discriminator
The discriminator network takes as input a 32x32 image and transforms it into a single valued probability of being generated from real-world data. Again we use tf.slim to define the convolutional layers, batch normalization, and weight initialization.

## Training

We trained the model on the MNIST database for 120 iterations and got the results shown below.

# Results

<img src="https://github.com/manumathewthomas/CS523P3PART1_DCGAN/blob/master/fig0.png" alt="alt text" width="600" height="320">

<img src="https://github.com/manumathewthomas/CS523P3PART1_DCGAN/blob/master/fig110.png" alt="alt text" width="600" height="320">
