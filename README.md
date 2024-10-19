# 😊 Facial Expression Classification with CNNs
## 🎯 Objective:
The goal of this project is to implement a Convolutional Neural Network (CNN) to classify facial expressions into seven distinct categories: Neutral, Happy, Sad, Surprise, Angry, Disgust, and Fear. This involves building and training the model, handling class imbalances, and evaluating the model's performance on a test dataset.

## 📝 Brief Description:
The code is divided into several key sections:

### 📊 Data Preprocessing:
This part handles:

Face Detection: Cropping faces using bounding box coordinates.
Resizing: All images are resized to 64x64 pixels.
Normalization: Pixel values are scaled for faster model convergence.
Class Imbalance Handling: Using SMOTE to address class imbalances.


### 🔄 Data Augmentation:
Techniques like rotation, zooming, shifting, and flipping are applied during training using the ImageDataGenerator in Keras to improve model generalization and prevent overfitting.



### 🧠 Model Architecture:
The CNN model consists of 5 convolutional layers, each followed by batch normalization, max pooling, and dropout layers for regularization. The fully connected layer has 1024 units, followed by a softmax layer for 7-class classification.



### 🏋️ Training and Evaluation:
The model is trained for 50 epochs, tracking training and validation loss and accuracy.
Evaluation: The test accuracy, confusion matrix, classification report, and F1 scores are generated.


### 📊 Visualization:
Visualizations include:

Training/Validation Accuracy and Loss Curves.
Confusion Matrix for classification performance analysis.
Displaying top-10 model predictions with their true labels.


### ✅ Conclusion:
The code successfully implements a CNN for facial expression classification. By combining SMOTE for class imbalance handling and data augmentation techniques, the model achieves over 65.5% accuracy on the test set. Future work could focus on fine-tuning the model or integrating it into real-time applications like emotion recognition in video streams.
