## The Rectified Linear Unit (ReLU)

In this lesson we talked about ReLU and how it gives our Dense layer more power. ReLU stands for Rectified Linear Unit and it is a mathematical function that looks like this:

![](image/tensorflow-l3f1.png)

As we can see, the ReLU function gives an output of 0 if the input is negative or zero, and if input is positive, then the output will be equal to the input.

ReLU gives the network the ability to solve nonlinear problems.

Converting Celsius to Fahrenheit is a linear problem because f = 1.8*c + 32 is the same form as the equation for a line, y = m*x + b. But most problems we want to solve are nonlinear. In these cases, adding ReLU to our Dense layers can help solve the problem.

ReLU is a type of activation function. There several of these functions (ReLU, Sigmoid, tanh, ELU), but ReLU is used most commonly and serves as a good default. To build and use models that include ReLU, you don’t have to understand its internals. But, if you want to know more, [see this article on ReLU in Deep Learning](https://www.kaggle.com/dansbecker/rectified-linear-units-relu-in-deep-learning).

Let’s review some of the new terms that were introduced in this lesson:

* Flattening: The process of converting a 2d image into 1d vector
* ReLU: An activation function that allows a model to solve nonlinear problems
* Softmax: A function that provides probabilities for each possible output class
* Classification: A machine learning model used for distinguishing among two or more output categories