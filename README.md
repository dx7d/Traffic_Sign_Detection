# Traffic Sign Detection with CNN

The main goal of this project is to develop a deep learning model capable of accurately classifying traffic signs from images.

## Table of Contents
1. [Importing Required Libraries](#importing-required-libraries)
2. [Assigning Path for Dataset](#assigning-path-for-dataset)
3. [Finding Total Classes](#finding-total-classes)
4. [Visualizing The Dataset](#visualizing-the-dataset)
5. [Collecting the Training Data](#collecting-the-training-data)
6. [Shuffling the Training Data](#shuffling-the-training-data)
7. [Splitting the Data into Train and Validation Sets](#splitting-the-data-into-train-and-validation-sets)
8. [CNN](#cnn)

## Importing Required Libraries

Various libraries are imported, including numpy, pandas, OpenCV (cv2), matplotlib, TensorFlow, Keras, and more. These libraries are used for data manipulation, visualization, machine learning model creation, and evaluation.

## Assigning Path for Dataset

The paths for the dataset's training and testing data are defined.

## Finding Total Classes

The number of classes (traffic sign categories) in the dataset is determined.

## Visualizing The Dataset

- The number of images in each class is visualized using a bar chart.
- A random selection of 25 test images is displayed in a 5x5 grid.

## Collecting the Training Data

- Training images and their corresponding labels are collected and preprocessed.
- Images are resized and appended to the `image_data` list, while labels are appended to the `image_labels` list.
- The data is converted to NumPy arrays.

## Shuffling the Training Data

The training data is shuffled randomly to ensure randomness during training.

## Splitting the Data into Train and Validation Sets

The data is split into training and validation sets using `train_test_split`.
The pixel values of the images are normalized to a range of 0 to 1.

## CNN

- A convolutional neural network (CNN) model is created using Keras.
- The model architecture includes convolutional layers, max-pooling layers, batch normalization, flattening, dense layers, and dropout.
- Data augmentation using `ImageDataGenerator` is applied during training.
- The model is trained, evaluated, and its performance metrics are displayed.

