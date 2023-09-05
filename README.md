# Emotion Detection using Convolutional Neural Networks

This repository contains code for building and training a Convolutional Neural Network (CNN) for emotion detection. The model is trained to recognize human emotions in facial images and classify them into one of seven categories: Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise. The code is designed to download a dataset from Kaggle and train a CNN model for this specific task.

## Installation

Before running the code, you'll need to install the required Python packages. You can do this using pip:

```
!pip install tensorflow opencv-python-headless
```

## Getting Started

To get started, follow these steps:

1. Clone this repository to your local machine.
2. Ensure you have the Kaggle API key available as `kaggle.json` in the root directory. You can obtain your API key from your Kaggle account settings.
3. Run the provided Jupyter Notebook or Python script to execute the code.

## Dataset

The dataset used in this project is the "Emotion Detection FER" dataset from Kaggle. The code will automatically download and unzip the dataset to the `/content` directory.

## Data Augmentation

Data augmentation techniques are applied to the images to enhance the model's ability to generalize. These techniques include random shifts, horizontal flips, and rescaling.

## Model Architecture

The CNN model architecture consists of multiple convolutional layers with batch normalization, max-pooling, and dropout layers to prevent overfitting. The model is designed to learn features from grayscale images with a size of 48x48 pixels.

## Training

The model is trained using the Adam optimizer with a learning rate of 0.0001 and categorical cross-entropy loss. Training is performed for 60 epochs. The training progress is visualized with training and validation accuracy and loss plots.

![image](https://github.com/devashishsagar/Emotion_Detection_Final_Project/assets/122087882/b3940d5b-014e-460f-bce3-a1dd64a9973f)


## Prediction

After training, the model can make predictions on new images. A sample image is loaded, preprocessed, and passed through the model to predict the emotion. The predicted emotion label is displayed along with the image.

![image](https://github.com/devashishsagar/Emotion_Detection_Final_Project/assets/122087882/b5ed0762-289f-4a23-9421-59496970a36a)


![image](https://github.com/devashishsagar/Emotion_Detection_Final_Project/assets/122087882/5a62d469-9a76-4b9a-bb61-14ac0e1b8330)

## Saving Model Weights

The trained model weights are saved to a file named `final_project_emotion_detection.h5` for future use.

Feel free to explore and modify the code as needed for your specific use case. If you have any questions or encounter any issues, please don't hesitate to reach out.
