# Cat and Dog Image Classifier

This project is a Convolutional Neural Network (CNN) built with TensorFlow 2.0 and Keras to classify images of cats and dogs. It was completed as part of the freeCodeCamp Machine Learning with Python certification.

## Project Goal
The objective of this challenge was to create a model that correctly identifies images of cats and dogs from a test set at least 63% of the time.

## Dataset Structure
The project uses a dataset organized into training, validation, and test directories:
* **train/**: Folders for cats and dogs used for training the model.
* **validation/**: Folders for cats and dogs used to tune the model and prevent overfitting.
* **test/**: A directory containing unlabeled images for final prediction.

## Model Implementation

### 1. Data Augmentation
To improve the model's performance and prevent overfitting, I used ImageDataGenerator to apply random transformations to the training data. These included:
* Rescaling (normalizing pixel values to a range of 0-1).
* Random rotations, shifts, shears, and zooms.
* Horizontal flips.

### 2. CNN Architecture
The model uses a Sequential architecture consisting of:
* Multiple Conv2D layers for feature extraction.
* MaxPooling2D layers to reduce spatial dimensions and parameter count.
* A Flatten layer to convert 2D feature maps into a 1D vector.
* A Dense layer with ReLU activation.
* A final Dense layer with a sigmoid activation to output binary probabilities (cat vs. dog).



### 3. Training
The model was compiled using the adam optimizer and binary_crossentropy loss function. It was trained for 15 epochs, tracking accuracy for both training and validation sets.

## How to Run
This project was developed locally using Jupyter Notebook.
1. Ensure you have TensorFlow, Numpy, and Matplotlib installed.
2. Download the project data from the link provided in the notebook.
3. Run the cells in the notebook to train the model and generate predictions.

## Final Results
Upon completion, the model passes the final test cell by reaching the required accuracy threshold of 63%.



---
Developed as part of the freeCodeCamp Machine Learning with Python Curriculum.
