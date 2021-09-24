## Recap

We just learned about convolutions and max pooling.

A convolution is the process of applying a filter (“kernel”) to an image. Max pooling is the process of reducing the size of the image through downsampling.

As you will see in the following Colab notebook, convolutional layers can be added to the neural network model using the Conv2D layer type in Keras. This layer is similar to the Dense layer, and has weights and biases that need to be tuned to the right values. The Conv2D layer also has kernels (filters) whose values need to be tuned as well. So, in a Conv2D layer the values inside the filter matrix are the variables that get tuned in order to produce the right output.

Here are some of terms that were introduced in this lesson:

* CNNs: Convolutional neural network. That is, a network which has at least one convolutional layer. A typical CNN also includes other types of layers, such as pooling layers and dense layers.
* Convolution: The process of applying a kernel (filter) to an image
* Kernel / filter: A matrix which is smaller than the input, used to transform the input into chunks
* Padding: Adding pixels of some value, usually 0, around the input image
Pooling The process of reducing the size of an image through downsampling.There are several types of pooling layers. For example, average pooling converts many values into a single value by taking the average. However, maxpooling is the most common.
* Maxpooling: A pooling process in which many values are converted into a single value by taking the maximum value from among them.
* Stride: the number of pixels to slide the kernel (filter) across the image.
* Downsampling: The act of reducing the size of an image