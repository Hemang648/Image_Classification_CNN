# Image_classification_CNN

## The dataset for this project is taken from here :- https://www.kaggle.com/datasets/kaustubhb999/tomatoleaf/discussion

## This script is a TensorFlow implementation for a tomato disease classification task using a convolutional neural network (CNN). Here's a breakdown of its functionality:

### 1. Data Preparation and Preprocessing:

* The script mounts Google Drive where the training data is stored.
* It lists the directories in the training data path, which represent different classes of tomato diseases.
* It defines a list of valid image extensions and removes corrupted images from the dataset based on these extensions.
* It creates a TensorFlow dataset from the directory containing the training images, with image resizing to 228x228 pixels.

### 2. Data Augmentation:

* Although not explicitly shown in the provided script, it includes commented-out code for data augmentation using ImageDataGenerator. Data augmentation techniques such as rescaling, shearing, zooming, and horizontal flipping are applied.

### 3. Model Building:

* The script constructs a CNN model using TensorFlow's Keras API. It defines a sequential model consisting of convolutional layers, max-pooling layers, flattening layers, dense layers, and dropout layers for regularization.
* The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss function.

### 4. Model Training:

* The model is trained using the fit method on the training dataset for a specified number of epochs, with validation data provided to monitor the model's performance.

### 5. Model Evaluation:

* The trained model is evaluated on the test dataset to compute its accuracy and loss.
### 6. Saving and Loading the Model:

* The script saves the trained model to Google Drive and later loads it for making predictions on new images.

### 7. Making Predictions:

* It demonstrates making predictions on new tomato images using the trained model. The input images are preprocessed and fed into the model to obtain predictions of the tomato diseases.

### 8. Post-prediction Analysis:

*Based on the predicted class index, the script provides explanations for each class, suggesting preventive measures and precautions for the identified diseases.

### 9. Visualization:

* The script includes code for visualizing the input images along with their predicted classes.

#### This script serves as a comprehensive pipeline for training a CNN model for tomato disease classification, including data preparation, model building, training, evaluation, and prediction. It also offers insights into the interpretation of model predictions and provides recommendations for disease management based on the predicted classes.
