# artificial_neural_network
Build and train a neural network to classify instances from a dataset using Keras, a high-level neural networks API.


 


Instructions

Dataset Options

Option : MNIST Dataset

Description: Comprises 28x28 pixel grayscale images of handwritten digits (0-9). This dataset is a good choice for those looking to work with image data, providing a balance of challenge and accessibility.
Data Loading and Preprocessing

## General Steps:

   * Normalize feature data.
   * Encode categorical labels.
   * Split the data into training and testing sets.
   * Reshape the 28x28 images into flat 784-pixel arrays.
   * Normalize pixel values to range between 0 and 1.
   * Convert labels into one-hot encoded vectors.
   * Optionally, create a validation set to aid in hyperparameter tuning.

## Model Building

### Configuration:

   * Input Layer: Adjust to match the number of input features (784 for MNIST, 4 for Iris).
   * Hidden Layers: Include at least one hidden layer with 'relu' activation. Additional layers may be added to increase model complexity.
   * Output Layer: Use 'softmax' activation for Iris and 'sigmoid' for binary classification tasks like MNIST (if treated as binary).

## Model Compilation

   * Optimizer: 'adam' for reliable performance across both datasets.
   * Loss Function: Use 'categorical_crossentropy' for multi-class tasks (both Iris and MNIST); 'binary_crossentropy' for binary classification.
   * Metrics: Focus on 'accuracy' as the primary metric.

## Model Training

   * Train the model using the training data, while utilizing the validation set to monitor performance.
   * Adjust training parameters such as epochs and batch size based on validation outcomes.

## Model Evaluation

   * Evaluate the model's performance using the test set.
   * Utilize detailed metrics such as the confusion matrix and classification report for more comprehensive insights.
