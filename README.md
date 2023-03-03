# WP1.3-Design-Parameters-Requirements

The program is now complete and ready to execute. After running the program, the model will be saved to a file called 'tf_model.h5' and the test accuracy of the model will be printed to the console.


To execute the program, you will need to have Python and TensorFlow installed on your computer. Once you have installed the necessary libraries, you will need to run the program using a Python interpreter. Depending on the platform you are using, this can be done in several different ways. For example, if you are using Windows, you can open the command line and type in 'python <program_name>.py' to execute the program. For more detailed instructions on running Python programs, please refer to the documentation for your platform.


The Python library that is used in the program is TensorFlow. TensorFlow is an open source library for numerical computation, developed by Google and used in many machine learning applications. It is available for download and installation from the official TensorFlow website.

1. Collect requirements from stakeholders, standard requirements, geometrical restrictions, customer feedback, and operating conditions.

2. Analyze the collected data to identify key design parameters for the circular blended wing concept aircraft model.

3. Develop a TensorFlow model that can simulate the performance of the aircraft model and validate it against the design parameters identified.

4. Use the TensorFlow model to test different design solutions and optimize them to meet the requirements and expectations of sustainable, efficient, and carbon neutral design.

5. Evaluate the performance of the optimized design solutions using the TensorFlow model and select the best one.

6. Specify the design parameters for the selected design solution.

7. Document the design parameters and the optimization process used.


The following python program can be used to execute a TensorFlow algorithm and produce a model from a given dataset:

# Import TensorFlow library
import tensorflow as tf

# Load the dataset
dataset = tf.keras.datasets.mnist

# Split the dataset into training and test sets
(train_images, train_labels), (test_images, test_labels) = dataset.load_data()

# Normalize the data
train_images = train_images / 255.0
test_images = test_images / 255.0

# Build the model
model = tf.keras.Sequential([
    tf.keras.layers.Flatten(input_shape=(28, 28)),
    tf.keras.layers.Dense(128, activation='relu'),
    tf.keras.layers.Dense(10, activation='softmax')
])

# Compile the model
model.compile(optimizer='adam',
              loss='sparse_categorical_crossentropy',
              metrics=['acc

please continue in full

# Train the model
model.fit(train_images, train_labels, epochs=5)

# Evaluate the model
test_loss, test_acc = model.evaluate(test_images, test_labels)

# Save the model
model.save('tf_model.h5')

print('Model saved!')

finish

# Print the results
print('Test accuracy:', test_acc)


