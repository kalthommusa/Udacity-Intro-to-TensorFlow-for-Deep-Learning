## Softmax and Sigmoid

In the previous Colab, we used the following the CNN architecture:

* model = tf.keras.models.Sequential([
    tf.keras.layers.Conv2D(32, (3,3), activation='relu', input_shape=(150, 150, 3)),
    tf.keras.layers.MaxPooling2D(2, 2),

    tf.keras.layers.Conv2D(64, (3,3), activation='relu'),
    tf.keras.layers.MaxPooling2D(2,2),

    tf.keras.layers.Conv2D(128, (3,3), activation='relu'),
    tf.keras.layers.MaxPooling2D(2,2),

    tf.keras.layers.Conv2D(128, (3,3), activation='relu'),
    tf.keras.layers.MaxPooling2D(2,2),

    tf.keras.layers.Flatten(),
    tf.keras.layers.Dense(512, activation='relu'),
    tf.keras.layers.Dense(2, activation='softmax')
])

Notice that our last layer (our classifier) consists of a Dense layer with 2 output units and a softmax activation function, as seen below:

     * tf.keras.layers.Dense(2, activation='softmax')

Another popular approach when working with binary classification problems, is to use a classifier that consists of a Dense layer with 1 output unit and a sigmoid activation function, as seen below:

     * tf.keras.layers.Dense(1, activation='sigmoid')

Either of these two options will work well in a binary classification problem. However, you should keep in mind, that if you decide to use a sigmoid activation function in your classifier, you will also have to change the loss parameter in the model.compile() method, from 'sparse_categorical_crossentropy' to 'binary_crossentropy', as shown below:

* model.compile(optimizer='adam', 
              loss='binary_crossentropy',
              metrics=['accuracy'])