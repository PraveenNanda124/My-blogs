# Artificial Intelligence (AI)

![a](https://user-images.githubusercontent.com/116082827/235301646-aad36230-85b6-47d1-a941-8257f111671c.jpeg)


AI involves creating intelligent machines that can perform tasks that typically require human intelligence, such as speech recognition, decision-making, and language translation. Here's an example of a simple AI program in Python that uses the Keras library to build a neural network for image classification:



import tensorflow as tf

from tensorflow import keras



# Load the dataset

(x_train, y_train), (x_test, y_test) = keras.datasets.mnist.load_data()



# Preprocess the data

x_train = x_train / 255.0

x_test = x_test / 255.0



# Build the model

model = keras.Sequential([

    keras.layers.Flatten(input_shape=(28, 28)),

    keras.layers.Dense(128, activation='relu'),

    keras.layers.Dense(10)

])



# Compile the model

model.compile(optimizer='adam',

              loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),

              metrics=['accuracy'])



# Train the model

model.fit(x_train, y_train, epochs=10)



# Evaluate the model

test_loss, test_acc = model.evaluate(x_test, y_test, verbose=2)

print('\nTest accuracy:', test_acc)
