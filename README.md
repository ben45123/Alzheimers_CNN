Alzheimer's Disease Classification: Predicting Alzheimer's disease stages using a convolutional neural network.

Overview:
This project aims to classify Alzheimer's disease stages based on brain scans using a convolutional neural network (CNN). The dataset used for training and testing the model contains brain scan images labeled with four stages of Alzheimer's disease: NonDemented, VeryMildDemented, MildDemented, and ModerateDemented.

Dataset:
The dataset used in this project consists of brain scan images stored in a directory structure. Each image is labeled with one of the following classes:

NonDemented
VeryMildDemented
MildDemented
ModerateDemented
The images are preprocessed and resized to (208, 176) pixels before being fed into the CNN model.

Model:
A CNN model is implemented using TensorFlow's Keras API. The model architecture includes convolutional layers, max-pooling layers, dropout regularization, and dense layers.

Training:
The dataset is split into training and testing sets. Data augmentation techniques are applied to augment the training dataset and prevent overfitting. The model is trained using the Adam optimizer with a categorical cross-entropy loss function. Early stopping is employed to prevent overfitting during training.

Results:
The trained model achieved an accuracy of 0.61 on the test set, improving upon the .56 accuracy of the most upvoted TensorFlow models on Kaggle. (Sources: https://www.kaggle.com/code/yassinabdulmahdi/alzheimer-s-best-model and https://www.kaggle.com/code/rudrashah003/alzheimer-s) The model demonstrates solid accuracy for classes with ample data, while also highlighting the impact of data scarcity on predictive capabilities for classes with minimal data.

Usage:
To use this model:

Download the provided Jupyter notebook (AlzheimerNeuralNetwork.ipynb) and the alzheimers dataset which can be found in the following link:
https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images/data?select=Alzheimer_s+Dataset

Run the notebook on platforms such as Google Colab or VSCode with TensorFlow and Keras installed.
Follow the instructions in the notebook to train and evaluate the model. Adjust hyperparameters or model architecture as needed for further experimentation.
