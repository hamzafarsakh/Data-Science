# Chest X-ray Image Classification with TensorFlow

## Introduction
This project focuses on building a Convolutional Neural Network (CNN) for classifying chest X-ray images into three categories: 'covid,' 'normal,' and 'pneumonia.' The goal is to develop an accurate and efficient model for assisting medical professionals in diagnosing chest conditions based on X-ray images.

## Dataset
The dataset used in this project consists of chest X-ray images obtained from various sources, including Kaggle. The images are organized into three subfolders corresponding to the three categories: 'covid,' 'normal,' and 'pneumonia.' 
Data Source: https://www.kaggle.com/datasets/amanullahasraf/covid19-pneumonia-normal-chest-xray-pa-dataset?resource=download

## Model Architecture
The model architecture utilized for this classification task is based on the InceptionV3 pre-trained CNN model. The InceptionV3 model is augmented with additional layers, including a Flatten layer, a Dense layer with ReLU activation, and a Dropout layer for regularization. Finally, a Dense layer with softmax activation is used as the output layer to predict the probabilities of each class.

## Data Preprocessing
The data preprocessing involves loading the images, resizing them to a standard size (96x96 pixels), and converting them into TensorFlow Dataset objects. The Dataset objects are then split into training, validation, and test sets. Additionally, data augmentation techniques such as shuffling and prefetching are applied to optimize dataset performance.

## Training
The model is trained using the training dataset with early stopping callbacks to prevent overfitting. The training progress is monitored using validation data to ensure the model's generalization capability. The training process aims to minimize the categorical cross-entropy loss function while maximizing accuracy metrics.

## Evaluation
The trained model is evaluated using both the validation and test datasets to assess its performance. Classification metrics such as accuracy, precision, recall, and F1-score are calculated and visualized using confusion matrices. The evaluation results provide insights into the model's ability to classify chest X-ray images accurately.

## Results
The InceptionV3-based CNN model achieves promising results in classifying chest X-ray images into 'covid,' 'normal,' and 'pneumonia' categories. The model demonstrates high accuracy and robustness, indicating its potential for real-world applications in medical diagnosis.

## Future Improvements
Future enhancements to this project could involve exploring different CNN architectures, hyperparameters tuning, and incorporating more advanced data augmentation techniques. Additionally, deploying the trained model as a web or mobile application for real-time chest X-ray image classification could further extend the project's impact in the medical field.
