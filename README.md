# Image-classification-using-CNN
This project implements a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset, consisting of 60,000 32x32 color images across 10 categories, such as airplanes, birds, and trucks. The project covers model development from scratch and explores several strategies to optimize model performance and reduce overfitting.

### Project Objectives
* Build a robust CNN model capable of classifying CIFAR-10 images.
* Apply data preprocessing, including normalization and one-hot encoding, to prepare the data.
* Implement regularization techniques to improve model generalization.

### Key Features
1. Model Architecture: Based on a VGG-like architecture, with three convolutional blocks, each followed by a max-pooling layer.
2. Data Augmentation: Employed real-time augmentation, including horizontal flips and shifts, to enhance training robustness.
3. Regularization:
   * Dropout Layers: Incremental dropout rates were used after each max-pooling layer and after the fully connected layer.
   * Batch Normalization: Added to each convolutional layer to stabilize learning and allow for higher learning rates.
4. Training and Evaluation: Utilized early stopping and data augmentation, training the model with 50 epochs and a batch size of 64.

### Usage
1. Clone this repository.
2. Load the CIFAR-10 dataset and preprocess it using the provided functions.
3. Define the CNN architecture and compile it with appropriate hyperparameters.
4. Train the model using the fit function, with early stopping and data augmentation.
