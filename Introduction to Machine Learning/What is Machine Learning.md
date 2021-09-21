## What is Machine Learning?

There are many types of neural network architectures. However, no matter what architecture you choose, the math it contains (what calculations are being performed, and in what order) is not modified during training. Instead, it is the internal variables (“weights” and “biases”) which are updated during training.

For example, in the Celsius to Fahrenheit conversion problem, the model starts by multiplying the input by some number (the weight) and adding another number (the bias). Training the model involves finding the right values for these variables, not changing from multiplication and addition to some other operation.

One cool thing to think about. If you solved the Celsius to Fahrenheit conversion problem you saw in the video, you probably did so because you had some prior knowledge of how to convert between Celsius and Fahrenheit. For example, you may have known that 0 degrees Celsius corresponds to 32 degrees Fahrenheit. On the other hand, machine learning systems never have any previous knowledge to help them solve problems. They learn to solve these types of problems without any prior knowledge.