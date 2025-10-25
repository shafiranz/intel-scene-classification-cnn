# Intel Scene Classification CNN
This project focuses on developing a Convolutional Neural Network (CNN) model using TensorFlow and Keras to classify natural scene images from the Intel Image Classification dataset. The dataset consists of six categories: buildings, forest, glacier, mountain, sea, and street.

The dataset was preprocessed by merging all images and splitting them into training, validation, and test sets to ensure balanced representation across classes. Image augmentation techniques such as rotation, zooming, shifting, and flipping were applied using the ImageDataGenerator to improve the model’s generalization and prevent overfitting.

The CNN architecture was built using the Sequential API with multiple Conv2D and MaxPooling2D layers, followed by dense layers for classification. The model was trained for 20 epochs with the Adam optimizer and early stopping to avoid overfitting.

After training, the model achieved strong performance:

1. Training Accuracy: 89.61%
2. Validation Accuracy: 87.56%
3. Test Accuracy: 86.40%

The trained model was successfully exported in three required formats:

1. SavedModel 
2. TensorFlow Lite 
3. TensorFlow.js 

Finally, inference testing on new, unseen images confirmed the model’s ability to predict the correct class — for instance, identifying a photo of a modern building as “buildings” with high confidence.
